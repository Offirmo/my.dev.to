---
title: Heroku pipelines: easy & free!
published: true
description: I tried heroku pipelines and it worked✔
tags: nodejs,heroku,backend,devops
---

Do you use heroku for your project's backend? You may be interested in setting up a **branch → staging → prod** pipeline. It's surprisingly easy!

My pet project uses an [Heroku](www.heroku.com) app as part of its backend.

ICYMI heroku is one of the simplest method to deploy a Node.js server with databases. And they have a good [free tier](https://www.heroku.com/pricing).

Heroku bugged me to upgrade my app from its outdated cedar-14 stack:

![Alt Text](https://dev-to-uploads.s3.amazonaws.com/i/d0kvrq9j72tnccbt13h5.png)

Instead of doing an upgrade, why not recreating it from scratch? And why not trying the pipeline feature?

An heroku pipeline is just an aggregation of "branch" → "staging" → "prod" apps, with the ability to promote an app to the next step. Setup:

1. create a pipeline, super easy through the UI
2. create (or add an existing) staging app
3. create (or add an existing) prod app
4. (I didn't use "review apps", too complicated for my simple setup)

The staging app then has a "promote to production" button:

![Alt Text](https://dev-to-uploads.s3.amazonaws.com/i/6k9f1q0p83q2zyp9fmhe.png)

which does what you guess = promote the staging app to prod.

Since I'm now using a single bolt monorepo for all my personal dev, I had to learn how to deploy an heroku app from a sub-package of a monorepo. Fortunately, [Laurent Grima](https://laugri.com) has us covered: [instructions](https://medium.com/inato/how-to-setup-heroku-with-yarn-workspaces-d8eac0db0256).

Once linked, I enabled auto-deploys on git push **for the staging app**.

Note that "promoting to production" doesn't means swapping the apps like in a blue-green deployment. It just means that the nodejs source will be copied over the target app. This is what we want since staging and prod have their own databases (through heroku app addons) that shouldn't be swapped.

I must now confess that I'm not really using heroku as a server... The free tier has a limited run time. I'm just using the free databases that can be attached to an app. They are always on and can be accessed from outside.

![Alt Text](https://dev-to-uploads.s3.amazonaws.com/i/ynf8rn7whyeuxuo757y0.png)
![Alt Text](https://dev-to-uploads.s3.amazonaws.com/i/cvnl3ykyavaxcp16yoc0.png)

My true server is powered by [Netlify functions](https://www.netlify.com/products/functions/) using a serveless architecture that I find much easier to reason about. The functions then access the heroku databases.

![Alt Text](https://dev-to-uploads.s3.amazonaws.com/i/1002id2ksgknxahq7jq8.png)

I was pleasantly surprised by the simplicity of heroku pipelines, I was expecting something much more complicated. Good job heroku!
