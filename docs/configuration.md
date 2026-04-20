---
title: Configuration
---

Quartz is meant to be extremely configurable, even if you don't know any coding. Most of the configuration you should need can be done by just editing `quartz.config.ts` or changing [[layout|the layout]] in `quartz.layout.ts`.

> [!tip]
> If you edit Quartz configuration using a text-editor that has TypeScript language support like VSCode, it will warn you when you you've made an error in your configuration, helping you avoid configuration mistakes!

The configuration of Quartz can be broken down into two main parts:

```ts title="quartz.config.ts"
const config: QuartzConfig = {
  configuration: { ... },
  plugins: { ... },
}
```

## General Configuration

This part of the configuration concerns anything that can affect the whole site. The following is a list breaking down all the things you can configure:

- `pageTitle`: title of the site. This is also used when generating the [[RSS Feed]] for your site.
- `pageTitleSuffix`: a string added to the end of the page title. This only applies to the browser tab title, not the title shown at the top of the page.
- `enableSPA`: whether to enable [[SPA Routing]] on your site.
- `enablePopovers`: whether to enable [[popover previews]] on your site.
- `analytics`: what to use for analytics on your site. Values can be
  - `null`: don't use analytics;
  - `cdnCaching`: if `true` (default), use Google CDN to cache the fonts. This will generally be faster. Disable (`false`) this if you want Quartz to download the fonts to be self-contained.
  - `typography`: what fonts to use. Any font available on [Google Fonts](https://fonts.google.com/) works here.
    - `title`: font for the title of the site (optional, same as `header` by default)
    - `header`: font to use for headers
    - `code`: font for inline and block quotes
    - body: font for everything  - colors: controls the theming of the site.
    - light: page background
    - lightgray: borders
    - gray: graph links, heavier borders
    - darkgray: body text
    - dark: header text and icons
    - secondary: link colour, current graph node
    - tertiary: hover states and visited graph nodes
    - highlight: internal link background, highlighted text, highlighted lines of code
    - textHighlight: markdown highlighted text background

Plugins

You can think of Quartz plugins as a series of transformations over content.



plugins: {
  transformers: [...],
  filters: [...],
  emitters: [...],
}


- Transformers map over content (e.g. parsing frontmatter, generating a description)
- Filters filter content (e.g. filtering out drafts)
- Emitters reduce over content (e.g. creating an RSS feed or pages that list all files with a specific tag)

You can customize the behaviour of Quartz by adding, removing and reordering plugins in the transformers, filters and emitters fields.


You should take care to add the plugin to the right entry corresponding to its plugin type. For example, to add the ExplicitPublish plugin (a Filter), you would add the following line:


filters: [
  ...
  Plugin.ExplicitPublish(),
  ...
],

To remove a plugin, you should remove all occurrences of it in the quartz.config.ts.

To customize plugins further, some plugins may also have their own configuration settings that you can pass in. If you do not pass in a configuration, the plugin will use its default settings.

For example, the Latex plugin allows you to pass in a field specifying the renderEngine to choose between Katex and MathJax.


transformers: [
  Plugin.FrontMatter(), // use default options
  Plugin.Latex({ renderEngine: "katex" }), // set some custom options
]


Some plugins are included by default in the quartz.config.ts, but there are more available.

You can see a list of all plugins and their configuration options here.

If you'd like to make your own plugins, see the making custom plugins guide.

Fonts

Fonts can be specified as a string or a FontSpecification:


// string
typography: {
  header: "Schibsted Grotesk",
  ...
}

// FontSpecification
typography: {
  header: {
    name: "Schibsted Grotesk",
    weights: [400, 700],

```ts title="quartz.config.ts"
plugins: {
  transformers: [...],
  filters: [...],
  emitters: [...],
}
```

- [[tags/plugin/transformer|Transformers]] **map** over content (e.g. parsing frontmatter, generating a description)
- [[tags/plugin/filter|Filters]] **filter** content (e.g. filtering out drafts)
- [[tags/plugin/emitter|Emitters]] **reduce** over content (e.g. creating an RSS feed or pages that list all files with a specific tag)

You can customize the behaviour of Quartz by adding, removing and reordering plugins in the `transformers`, `filters` and `emitters` fields.

> [!note]
> Each node is modified by every transformer _in order_. Some transformers are position sensitive, so you may need to pay particular attention to whether they need to come before or after certain other plugins.

You should take care to add the plugin to the right entry corresponding to its plugin type. For example, to add the [[ExplicitPublish]] plugin (a [[tags/plugin/filter|Filter]]), you would add the following line:

```ts title="quartz.config.ts"
filters: [
  ...
  Plugin.ExplicitPublish(),
  ...
],
```

To remove a plugin, you should remove all occurrences of it in the `quartz.config.ts`.

To customize plugins further, some plugins may also have their own configuration settings that you can pass in. If you do not pass in a configuration, the plugin will use its default settings.

For example, the [[plugins/Latex|Latex]] plugin allows you to pass in a field specifying the `renderEngine` to choose between Katex and MathJax.

```ts title="quartz.config.ts"
transformers: [
  Plugin.FrontMatter(), // use default options
  Plugin.Latex({ renderEngine: "katex" }), // set some custom options
]
```

Some plugins are included by default in the [`quartz.config.ts`](https://github.com/jackyzha0/quartz/blob/v4/quartz.config.ts), but there are more available.

You can see a list of all plugins and their configuration options [[tags/plugin|here]].

If you'd like to make your own plugins, see the [[making plugins|making custom plugins]] guide.

## Fonts

Fonts can be specified as a `string` or a `FontSpecification`:

```ts
// string
typography: {
  header: "Schibsted Grotesk",
  ...
}

// FontSpecification
typography: {
  header: {
    name: "Schibsted Grotesk",
    weights: [400, 700],
    includeItalic: true,
  },
  ...
}
```
