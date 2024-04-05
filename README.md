# Create T3 App

This is a [T3 Stack](https://create.t3.gg/) project bootstrapped with `create-t3-app`.

## What's next? How do I make an app with this?

We try to keep this project as simple as possible, so you can start with just the scaffolding we set up for you, and add additional things later when they become necessary.

If you are not familiar with the different technologies used in this project, please refer to the respective docs. If you still are in the wind, please join our [Discord](https://t3.gg/discord) and ask for help.

- [Next.js](https://nextjs.org)
- [NextAuth.js](https://next-auth.js.org)
- [Prisma](https://prisma.io)
- [Drizzle](https://orm.drizzle.team)
- [Tailwind CSS](https://tailwindcss.com)
- [tRPC](https://trpc.io)

## Learn More

To learn more about the [T3 Stack](https://create.t3.gg/), take a look at the following resources:

- [Documentation](https://create.t3.gg/)
- [Learn the T3 Stack](https://create.t3.gg/en/faq#what-learning-resources-are-currently-available) — Check out these awesome tutorials

You can check out the [create-t3-app GitHub repository](https://github.com/t3-oss/create-t3-app) — your feedback and contributions are welcome!

## How do I deploy this?

Follow our deployment guides for [Vercel](https://create.t3.gg/en/deployment/vercel), [Netlify](https://create.t3.gg/en/deployment/netlify) and [Docker](https://create.t3.gg/en/deployment/docker) for more information.

this should show up as a change

important commands upon setup to run:

cd something
npx prisma generate
npx prisma db pull --force
npm run db:push
npm run dev
git init
git commit -m "initial commit"
npx prisma studio - this is to manually add data into the db

ThisShouldBeStronger12

Notes on Routing

When using React their are two types of routing systems that occur. Their is server side routing and client side routing. Server side routing is when the server takes in a request and returns the following javascript and html that was expected from a certain route. Client side routing occurs when you have content already but you want to change a page. Instead of rerendering everything it only fetches the things it needs and the client side handles the routing and how things are displayed.
[9:51 PM]
I think a good demonstration of something like this happening is the react-router, vs something like django handling routing.

react router if you hit the refresh button on a page you will be sent a 404 page because that route does not exist on the server, but if you click on the nav button of the website you can get their. That has to deal with the content being sent all at once to the client and then the client displays what is needed for each view.
[9:53 PM]
django it you hit a refresh page and page was a valid page your page will always rerender, nomatter what. That is because that is a valid route on the server, but the downside is that client side has no routing system so every page requires a hit to the server which could cause some performance issues depending on what you are doing. Also more resources are needed for each request because you may be sending redundant info like the nav bar