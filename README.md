## Make JAMstack apps, not sites with Gatsby + Netlify Identity + Netlify Functions

This is a fork of https://github.com/gatsbyjs/gatsby-starter-default which shows how to use Netlify Identity and Netlify Functions with Gatsby. Start here for your next JAMstack hackathon or use this as a reference implementation.

[![Netlify Status](https://api.netlify.com/api/v1/badges/ce755967-ad26-4a80-99b5-1349b58d2c07/deploy-status)](https://app.netlify.com/sites/goofy-fermat-d94d9f/deploys)

## 3 minute video walkthrough

[![walkthru](https://img.youtube.com/vi/bueXJInQt2c/1.jpg)](https://www.youtube.com/watch?v=bueXJInQt2c)

## Make your own from scratch!

Check our post on the Gatsby blog: [Turning the Static Dynamic: Gatsby + Netlify Functions + Netlify Identity](https://www.gatsbyjs.org/blog/2018-12-17-turning-the-static-dynamic/)

## How to start

You can clone and deploy this sample project with one click:
[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/sw-yx/jamstack-hackathon-starter&stack=cms)

Basically these are the extra dependencies it adds:

- [`netlify-lambda`](https://github.com/netlify/netlify-lambda): For locally emulating Netlify Functions
- `http-proxy-middleware`: For proxying netlify-lambda function calls to avoid CORS issues as [per the Gatsby docs](https://www.gatsbyjs.org/docs/api-proxy/#advanced-proxying)
- [`netlify-identity-widget`](netlify-identity-widget): For adding

## Enabling Netlify Identity

If you are not using the **Deploy to Netlify** button (which has the `&stack=cms` parameter that automatically sets it up for you), you will have to enable Netlify Identity manually yourself. Just head to `https://app.netlify.com/sites/YOUR_SITE_HERE/identity` and enable it, so that your `netlify-identity-widget` works.

## Further Documentation in nested READMEs

- please see the [src README](/src/README.md) for explanation on the layout
- please see the [app README](/src/app/README.md) for explanation on the app

## Other Resources

Other useful resources/reference projects that may help you:

- https://github.com/netlify/create-react-app-lambda
- https://github.com/netlify/netlify-identity-widget/tree/master/example

Please contact [@swyx](https://twitter.com/swyx) if you need more help with Netlify.
