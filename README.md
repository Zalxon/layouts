
# zalxon / layouts

**page layout components for documents and tools**

[![GitHub][github-badge]][github]
[![Build Status]][actions]
![MIT License][]
![NPM Version][]

[github]: https://github.com/zalxon/layouts
[github-badge]: https://badgen.net/badge/-/github?icon=github&label
[build status]: https://github.com/zalxon/layouts/actions/workflows/main.yml/badge.svg
[actions]: https://github.com/zalxon/layouts/actions/workflows/main.yml
[mit license]: https://badgen.net/badge/license/MIT/blue
[npm version]: https://badgen.net/npm/v/@zalxon/layouts

Reusable [`react`](https://github.com/facebook/react) components for common layouts, such as those used in our articles, tools, blog posts, and maps. All the components here either wrap the base `Layout` from `@zalxon/components` directly, or are linked in their design constraints to one of the layouts in this package that do so. Similar to those in the [`@zalxon/components`](https://github.com/zalxon/components) package, these components assume and make extensive use of [`theme-ui`](https://github.com/system-ui/theme-ui) and [`next`](https://github.com/vercel/next.js), and are meant to be composed with our [`theme`](https://github.com/zalxon/theme). These components also work particularly well with MDX, which we use for authoring lots of our content.

## usage

To use, install the package with

```
npm i @zalxon/layouts
```

and then import the component(s) you want into your `next` project.

## examples

The easiest way to understand these components is to see them in use across our sites.

- Visit [zalxon.com/research](https://zalxon.com/research) or [github.com/zalxon/research](https://github.com/zalxon/research) to see the use of `Article` and `Tool`.
- Visit [zalxon.com/blog](https://zalxon.com/blog) or [github.com/zalxon/blog](https://github.com/zalxon/blog) to see the use of `Post`.
- Visit [zalxon.com/design](https://zalxon.com/design) or [github.com/zalxon/design](https://github.com/zalxon/design) to see the use of `NavSection` and `NavMenu`.

## api

Most of these components are wrappers for the [`Layout`](https://github.com/zalxon/components/blob/main/src/layout.js) component that we generally use as the top-level component for our pages. As such, they are also intended to act as top-level page components. In particular, `Article` `Supplement` `Post` `Tool` and `NavSection` all play this role.

The remaining components are either elements of those layouts that might sometimes be useful on their own, llike `NavMenu`, or components that se only in the context of these layouts and are linked via specifid design constraints, like the use of `Cite` and `PullQuote` within an `Article`.

Here are all the components currently available, grouped by where we tend to use them (some components appear in multiple groups):

### research articles

`Article`
`Supplement`
`Endnote`
`Cite`
`PullQuote`
`Sidenote`

### interactive tools

`Tool`

### blog posts

`Post`

### documentation sites

`NavSection`
`NavMenu`

### tool sites

`Sidebar`
`SidebarAttachment`
`SidebarFooter`
`SidebarDivider`
