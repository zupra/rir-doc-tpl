# Documentation Site Template

This template is a paired down version of [Cleavr's documentation website](https://docs.cleavr.io) that you can use as a starter template for your own documentation website. 

You can check out the [docs template live preview](https://docstemplate.cleavr.cloud) to view and interact with the template. 

## Details

The template uses NuxtJS and relies on their Content module. Additional libraries used for the template can be found on the [live preview](https://docstemplate.cleavr.cloud) landing page. 

Feel free to fork this project and make your own. 

Check out the accompanying tutorial series - 

[dev.to turial series](https://dev.to/armiedema/getting-started-with-nuxtjs-content-module-3l5o)

[YouTube playlist series](https://www.youtube.com/watch?v=OvtgcS6RL2Y&list=PLApnZzwJN4G5jU3NzBPWpHWJiXTEO9esd)

## Setup for local environment

```bash
# install dependencies
$ yarn install

# serve with hot reload at localhost:3000
$ yarn dev
```

## Algolia Search

If you use the Algolia Search feature, the index will be created and delivered to your Algolia account during the site generation step for static sites. 

This template has Nuxt Static site generation enabled; however, you can configure to run in SSR mode if you prefer. Though, you'd need to find a different method to compile your index for Algolia as the package plugin requires that static site generation to run. 

---

[<img src="https://docs.cleavr.io/images/deploy-with-cleavr.png" height="25px"/>](https://cleavr.io/flash?vc-profile=e8d5603c-78ff-49f2-b6cf-badfbdec7aae&webapp=nuxtStatic&repository=cleavr/docs-template&branch=master&vps-region=sfo2&db-server=mysql57&vps-provider=digitalocean&vc-provider=github&vps-plan=s-1vcpu-1gb&flash=true)
