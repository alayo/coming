# Installation

After downloading the file from Themeforest, You will find Deadline.zip file. Then unzip the Deadline.zip and run the following commands on Deadline folder to get started with the project.

```
yarn
```

```
// For starting NextJs Server run
yarn nextjs-dev
```

NextJs Server will start in `localhost:3000`

Available routes are below

```
/one
/two
/three
/four
/five
/six
/seven
/eight
/nine
/ten
/elevel
/twelve
/thirteen
/fourteen
/fifteen
/sixteen
/seventeen
/eighteen
/nineteen
/twenty
/twenty-one
/twenty-two
```

<br/><br/><br/><br/><br/><br/>

# Folder Structure

```
/common [All the common resource throughout the project]
	/data
		/social-share
		/translation
	/demoSwitcher
	/hooks
	/LanguageSwitcher
	/static
	/theme
	/ui
/components [Components throughout the project ]
/nextjs [NextJs dependend component, pages and containers]
```

# Development

Follow the below procedure to go with the development process.

## NextJs

If you want to develop only for gatsbyjs then then you don't need the `/gatsbyjs` folder. You can delete the folder.

Follow the same steps for nextjs on `/nextjs` folder. Except starting the server for nextjs you have to run `yarn nextjs-dev` and the server will start on `locahost:3000`.

# Data

Theres two folders in `/common/data` folder

### /social-share

`/social-share` folder contains template specific social share data like `/social-share/one.js` contains data for `/pages/one.js` template

### /translation

In this folder, you will find all the translations that we have used in our template . We have used `react-intl` (https://github.com/formatjs/react-intl) to Internationalise our template . You can translate the template into any language you want. We have already given support for 6 languages. They are English(en), Arabic(ar), German(de), Spanish(es), Chinese(zh) and Hebrew(he).

We have also provided Right to Left(RTL) alignment supports.

# SendGrid Integration

We have provided support for SendGrid (https://sendgrid.com/) integration for email delivery/ Newsletter/ Contact form.

<br/><br/><br/><br/><br/><br/>

## NextJs

1. Go to , `/nextjs/next.config.js` find the code section and put your SendGrid Api Key there.

```
const nextConfig = {
	env: { SENDGRID_API_KEY: 'Put your SendGrid Api Key here' }
}
```

NOTE: We have commented out the sendgrid implementation, you will able to use that code that way or you can run separate node js server to send it to your sendgrid. it's upto you.

# Deployment

For deploying your final project you have to build your project first. To build the project you have to follow below procedure.

### NextJs Build

To build the nextjs version run below commands.

```
yarn nextjs-build

// To check the build version locally run below command
// Not necessary if you don't want to check on your local.
yarn nextjs-serve
```

<br/><br/><br/><br/><br/><br/><br/><br/>

## Deployment Support

```

### NextJs on Vercel

For deploying nextjs on now.sh you have rename `next.vercel.json` to `vercel.json`. Now run below command after building the project.

```

vercel

```

> **Make sure you have `vercel-cli` installed in your system.**
```
