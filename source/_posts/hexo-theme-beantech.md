---
title: "[Hexo] Theme BeanTech"
catalog: true
date: 2017-03-18 10:51:24
subtitle: "This is hexo theme Demo."
header-img: "Demo.png"
tags:
- Hexo
- Blog
catagories:
- Hexo
---
> Ported Theme of [Hux Blog](https://github.com/Huxpro/huxpro.github.io), Thank [Huxpro](https://github.com/Huxpro) for designing such a flawless theme.
> 
> This BeanTech theme modified from the original Porter [Kaijun](http://kaijun.rocks/hexo-theme-huxblog/)

# [Live Demo](http://beantech.org)
---
![BeanTech Desktop](http://beantech.org/img/beantech-desktop.png)

# Usage
---
I didn't publish it as a single theme folder because a few of the pages are added and modified manually, so you should manually create some extra folders in `source` for the new pages and modify the `_config.yml` if you only have the single theme folder.

So i just pushed the whole hexo project for your convenience, all pre settings and boilerplates are included, have a look and go ahead customizing your own blog!

## Init
---
```bash
git clone https://github.com/YenYuHsuan/hexo-theme-beantech.git ./hexo-beantech
cd hexo-beantech
npm install
```

## Modify
---
Modify `_config.yml` file with your own info.
Especially the section:
### Deployment
Replace to your own repo!
```yml
deploy:
  type: git
  repo: https://github.com/<yourAccount>/<repo>
  branch: <your-branch>
```

### Sidebar settings
Copy your avatar image to `<root>/img/` and modify the `_config.yml`:
```yml
sidebar: true    # whether or not using Sidebar.
sidebar-about-description: "<your description>"
sidebar-avatar: img/<your avatar path>
```
and activate your personal widget you like
```yml
widgets:         # here are widget you can use, you can comment out
- featured-tags
- short-about
- recent-posts
- friends-blog
- archive
- category
```
if you want to add sidebar widget, please add at `layout/_widget`.
### Signature Setup
Copy your signature image to `<root>/img/signature` and modify the `_config.yml`:
```yml
signature: true   # show signature
signature-img: img/signature/<your-signature-ID>
```
### Go to top icon Setup
My icon is using iron man, you can change to your own icon at `css/image`.

## Writting/ Server / Deploy
---
Some hexo command:
```bash
hexo new post "<post name>" # you can change post to another layout if you want
hexo clean && hexo generate # generate the static file
hexo server # run hexo in local environment
hexo deploy # hexo will push the static files automatically into the specific branch(gh-pages) of your repo!
```
# Enjoy! 
---
Please [**Star**](https://github.com/YenYuHsuan/hexo-theme-beantech/stargazers) this Project if you like it! [**Follow**](https://github.com/YenYuHsuan) would also be appreciated!
Peace!
