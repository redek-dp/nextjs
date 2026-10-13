
Como hospedar um app NextJS no Github Pages

https://nextjs.org/docs/app/guides/static-exports

```bash

next.config.js

/**
 * @type {import('next').NextConfig}
 */
const nextConfig = {
    output: 'export',

    distDir: 'dist',
    images: {
        unoptimized: true,
    },
}

module.exports = nextConfig;

```


https://racoelho.com.br/posts/como-hospedar-um-app-nextjs-no-github-pages


```bash

npx create-next-app@latest

cd blog-starter-app

npm run dev

npm run build

npx serve ./dist

```