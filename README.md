## Tiny vercel proxy

### By deploying your code (or running it locally with npm start) any call made to the /api endpoint will be proxied to https://example.org.

Check the documentation of the http-proxy-middleware library (and of the node-http-proxy library, used under-the-hood) to learn how you can manipulate the proxied request & response.

## Deploy on your own Vercel instance

#### [Check Out Step By Step Video Tutorial By @codeSTACKr](https://youtu.be/n6d4KHSKqGk?t=107)

Since the GitHub API only allows 5k requests per hour, my `https://github-readme-stats.vercel.app/api` could possibly hit the rate limiter. If you host it on your own Vercel server, then you don't have to worry about anything. Click on the deploy button to get started!

NOTE: Since [#58](https://github.com/anuraghazra/github-readme-stats/pull/58) we should be able to handle more than 5k requests and have no issues with downtime :D

[![Deploy to Vercel](https://vercel.com/button)](https://vercel.com/import/project?template=https://github.com/anuraghazra/github-readme-stats)

<details>
 <summary><b> Guide on setting up Vercel  🔨 </b></summary>

1. Go to [vercel.com](https://vercel.com/)
1. Click on `Log in`
   ![](https://files.catbox.moe/tct1wg.png)
1. Sign in with GitHub by pressing `Continue with GitHub`
   ![](https://files.catbox.moe/btd78j.jpeg)
1. Sign in to GitHub and allow access to all repositories, if prompted
1. Fork this repo
1. After forking the repo, open the [`vercel.json`](https://github.com/anuraghazra/github-readme-stats/blob/master/vercel.json#L5) file and change the `maxDuration` field to `10`
1. Go back to your [Vercel dashboard](https://vercel.com/dashboard)
1. Select `Import Project`
   ![](https://files.catbox.moe/qckos0.png)
1. Select `Import Git Repository`. Select root and keep everything as is.
   ![](https://files.catbox.moe/pqub9q.png)
1. Create a personal access token (PAT) [here](https://github.com/settings/tokens/new) and enable the `repo` permissions (this allows access to see private repo stats)
1. Add the PAT as an environment variable named `PAT_1` (as shown).
   ![](https://files.catbox.moe/0ez4g7.png)
1. Click deploy, and you're good to go. See your domains to use the API!

</details>

## :sparkling_heart: Support the project

I open-source almost everything I can, and I try to reply to everyone needing help using these projects. Obviously,
this takes time. You can use this service for free.

However, if you are using this project and are happy with it or just want to encourage me to continue creating stuff, there are a few ways you can do it:-

- Giving proper credit when you use github-readme-stats on your readme, linking back to it :D
- Starring and sharing the project :rocket:
- [![paypal.me/anuraghazra](https://ionicabizau.github.io/badges/paypal.svg)](https://www.paypal.me/anuraghazra) - You can make one-time donations via PayPal. I'll probably buy a ~~coffee~~ tea. :tea:

Thanks! :heart:

---

[![https://vercel.com?utm_source=github_readme_stats_team&utm_campaign=oss](./powered-by-vercel.svg)](https://vercel.com?utm_source=github_readme_stats_team&utm_campaign=oss)

Contributions are welcome! <3

Made with :heart: and JavaScript.
