# nextjs
Learn next js 

# Getting Started

<code>create-next-app</code>

cli to create Next.js application using default template

```bash
npx create-next-app@latest [project-name] [options]
```

# Rendering Strategies

<p>Determine how application user interface is generated and delivered.</p>

<span>Provide vaying trade-off</span>
<ol>

<li>Performance</li>
<li>SEO</li>
<li>Data freshness</li>

</ol>

> Note: Choosing right rendering strategy is important for optimizing application based on requirement.

> Summary:
> <li>Important thing for SEO - page data and metadata available on page load without js</li>
> <li>Rendering methods can be done on page basis</li>

## Static Site Generation (SSG)
<span>
HTML generated at build time. Then this is used for every request. Best rendering strategy for SEO - 
    <li>All HTML elements on page load.</li>
    <li>Helps with page performance.</li>
</span>

## Server-Side Rendering (SSR)
<span>
Same as SSG, great for SEO. But HTML is generated at request time. Great for pages that are very dynamic.
</span>

## Incremental Static Regeneration (ISR)
<span>
    If large amount of pages SSG is not feasible. NextJS allows to create ot update static pages after site built. With ISR, retain the benefit of static while scaling to millions of pages.
</span>

## Client Side Rendering (CSR)
<span>
    Entirely rendered on client side with js. Not recommened for SEO. Recommened for data heavy dashboards, account pages or any pages that do not require to be in any search engine index.
</span>

# Reference doc

1. [Getting started](https://nextjs.org/docs/app/api-reference/cli/create-next-app)
2. [Next.js Rendering Strategies: SSR, SSG, and ISR Compared](https://hybridheroes.de/blog/2023-05-31-next-js-rendering-strategies/)