Como hospedar um app NextJS no Github Pages

https://nextjs.org/docs/app/guides/static-exports

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


https://racoelho.com.br/posts/como-hospedar-um-app-nextjs-no-github-pages

cd blog-starter-app

npm run dev

npm run build

npx serve ./dist