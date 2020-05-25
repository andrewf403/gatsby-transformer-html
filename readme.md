*Added*: url slug, full text, html not constrained to <article>, other changes

*Added*: section info to the frontmatter based on *very* specific file naming convention.

```
DocumnetName.01.02.html
             ^------------- sectionNumber
                 ^--------- articleNumber
             ^____^
                |---------- documentNumber
```

*Added*: Removing of *very* specific `no script` leftovers

*Added*: `excerpt` of 100 chars (should be an option, really)

Based on: 
A Gatsby transformer plugin for authoring content in HTML, part of
[`gatsby-starter-apidocs`](https://github.com/carrotsearch/gatsby-starter-apidocs).

---

One functional area of the plugin is enriching raw HTML content by:

* rewriting local links to point to the generated Gatsby pages,

* adding section anchor links,

* processing linked images into multi-resolution responsive img tags,

* applying Prism.js highlighting to code blocks,

* embedding code examples from external files,

* adding synthetic identifiers to paragraph to make it possible to link to them from content search results.

Another functional area of the plugin is extracting paragraph-sized text snippets from the page, so that they can be indexed in the client-side text search implemented by the [`gatsby-plugin-content-search`](https://github.com/carrotsearch/gatsby-plugin-content-search) plugin.

The enriched HTML and lists of extracted text snippets are available in Gatsby's GraphQL model for use by other plugins.


License: MIT

