## Setup
``` npx create-next-app@latest```
- Install dependencies ```npm install @headlessui/react @heroicons/react date-fns --save```
- Install tailwind plugins ```npm install -D @tailwindcss/aspect-ratio @tailwindcss/typography @tailwindcss/forms```
- In tailwind.config.js, add the required plugins
```
require('@tailwindcss/aspect-ratio'),
require('@tailwindcss/forms'),
require('@tailwindcss/typography')
```
- Then run the app ```npm run dev```
- Components are Server Components by default. For Client Component, you shall mark as a client entry with "use client"

## Notes
- In case the { products } returned is undefined, you can first test to see if the API endpoint and access key are correct. You can also use a try-catch to make sure the API is returned and figured out what is the actually cause.
- This project is set to no app.js initiated because of the getStaticProps, which cannot be used in the app itself   

## About Next.js
This is a [Next.js](https://nextjs.org/) project bootstrapped with [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app).

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.js`. The page auto-updates as you edit the file.

This project uses [`next/font`](https://nextjs.org/docs/basic-features/font-optimization) to automatically optimize and load Inter, a custom Google Font.

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js/) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/deployment) for more details.
