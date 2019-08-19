<p align="center">
  <a style="padding-right: 16px;" href="https://forestry.io">
    <img src="https://app.forestry.io/assets/forestry-logotype-pos-c71a6bd237d9199d0457ba2811553997ff5bab0d2cd0e740686ab26c00d9c240.svg" width="112" height="28">
  </a>
  <a href="https://gohugo.io/">
    <img src="/static/hugo-logo-wide.svg" width="112" height="28">
  </a>
</p>
<h1 align="center">
  Brevifolia
</h1>

## About

Brevifolia is minimalist blog starter to get you going using [Forestry](https://forestry.io/) with [Hugo](https://gohugo.io/). See the demo [here](https://brevifolia-forestry-hugo.netlify.com/)

This blog is statically generated by Hugo. It is preconfigured to work with Forestry as a way to manage your content. Forestry makes changes by editing markdown or data files, uploading media to the correct directory and committing these updates to your repo directly.

The Hugo version of this Brevifolia starter was built upon the already well-known [Tale Theme](https://github.com/EmielH/tale-hugo). The ammended styles were coded & designed by yours truly, using [scss](https://sass-lang.com/) and the [bem](http://getbem.com/) naming convention. The font used is [Work Sans](https://fonts.google.com/specimen/Work+Sans). 

##  Quick Setup

#### *Import to Forestry Button*

<a href="https://app.forestry.io/quick-start?repo=kendallstrautman/starter-blog-hugo&engine=hugo&version=0.57.2&config=site">
    <img alt="Import this project into Forestry" src="https://assets.forestry.io/import-to-forestryK.svg" />
</a>

#### *Set-up Locally*
In your terminal, navigate to where you would like this blog to live, then run 
```bash
#clone the repo
git clone git@github.com:kendallstrautman/starter-blog-hugo.git

#navigate to the directory
cd starter-blog-hugo

#install dependencies & run dev server with yarn 
yarn install
hugo serve

#or with npm 
npm install
hugo serve
```
A new browser window should open with the dev server running or you can navigate to localhost:8000 

## Project Structure 

- Site-level configuration is stored in `config.toml`, this is required in the root for Forestry to setup the project. 
- Edit styles via `themes/assets/scss/tale/...`
- `content/...`contains all your markdown blog posts, pages & data files (e.g. authors list, info page data). 
- Images and media are uploaded to `static/images/...`
- Templates can be edited in `themes/layouts/...`

## Using Forestry as your CMS

The `.forestry` directory contains all the settings information and frontmatter configuration to allow Forestry to setup the sidebar structure and editing capacity for this blog. After importing this blog into forestry, you can [access and edit](https://forestry.io/docs/editing/) all of the content via the sidebar. 

You can add new blog posts, [data files](https://forestry.io/docs/editing/data-files/), or entire pages and sections to fit your needs. You can also [customize how media](https://forestry.io/docs/media/) is handled, by configurating gitLFS, Cloudinary, S3, or Netlify Large Media.

You can set up a [remote admin](https://forestry.io/docs/editing/remote-admin/) for content editors to log in directly to yoururl.com/admin to make content updates.

### Instant Previews

The [instant preview](https://forestry.io/docs/previews/instant-previews/) method spins up a development server for a long-lived preview that can quickly respond to content updates. When using instant previews, your preview command should be the develop command. The development server spawned by this command should be available over port 8080, and bind to 0.0.0.0.

## Deploy Options

[Netlify](https://www.netlify.com/blog/2016/09/29/a-step-by-step-guide-deploying-on-netlify/) is a great way to easily deploy sites. There's no special setup you need to do with Forestry to deploy with Netlify. When Forestry makes commits to your repo, Netlify will auto-trigger a rebuild / deploy when new commits are made.
