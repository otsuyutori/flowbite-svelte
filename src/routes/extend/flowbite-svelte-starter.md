---
layout: pageLayout
breadcrumb_title: Starter
title: Flowbite-Svelte Starter
dir: Extend
---


<MetaTags
  title={breadcrumb_title}
  titleTemplate="%s | Flowbite-Svelte"
  description={title}
  openGraph={{
    title: `${title}`,
    description: `${title}`,
    images: [
      {
        url: `https://open-graph-vercel.vercel.app/api/flowbite-svelte?title=${breadcrumb_title}`,
        width: 800,
        height: 600,
        alt: `${title}`
      }
    ],
    site_name: 'Flowbite-Svelte'
  }}
  twitter={{
    handle: '@shinokada',
    cardType: 'summary_large_image',
    title: `${title}`,
    description: `${title}`,
    image: `https://open-graph-vercel.vercel.app/api/flowbite-svelte?title=${breadcrumb_title}`,
    imageAlt: `${title}`
  }}
/>

<script>
  import Htwo from '../utils/Htwo.svelte'
  import { MetaTags } from 'svelte-meta-tags';
  import { Breadcrumb, BreadcrumbItem, Heading, A } from '$lib'
</script>

<Breadcrumb class="pt-16 py-8">
  <BreadcrumbItem href="/" home >Home</BreadcrumbItem>
  <BreadcrumbItem>{dir}</BreadcrumbItem>
  <BreadcrumbItem>{breadcrumb_title}</BreadcrumbItem>
</Breadcrumb>

<Heading class="mb-2" tag="h1" customSize="text-3xl">{title}</Heading>

<Htwo label="Demo" />

<p class="dark:text-white" ><a class="text-blue-700" href="https://flowbite-svelte-starter.vercel.app/">Flowbite-Svelte-Starter Demo</a></p>

<Htwo label="Features" />

<ul class="dark:text-white">
<li>Svelte</li>
<li>SvelteKit</li>
<li>Tailwind CSS</li>
<li>Flowbite</li>
<li>Flowbite-Svelte</li>
<li>Flowbite-Svelte-Blocks</li>
<li>ESlint</li>
<li>Typescript</li>
<li>Playwright</li>
<li>Prettier</li>
<li>Svelte-heros(Heroicons)</li>
<li>Darkmode activated</li>
</ul>

<Htwo label="Installation" />

```sh
npx degit shinokada/flowbite-svelte-starter my-demo
cd my-demo
pnpm i // or npm i
pnpm run dev // or npm run dev
```

<Htwo label="Other examples/themes" />

<Htwo label="Svelte-Sidebar-Example" />

If you want to see [a svelte-sidebar demo](https://flowbite-svelte-starter.vercel.app/):

```sh
git checkout svelte-sidebar-example
```

<Htwo label="Jaco example" />

```sh
git checkout jaco
```

<Htwo label="Plain" />

```sh
git checkout plain
```
