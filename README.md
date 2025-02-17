# annawilde.github.io

This repository is the code base for the professional website of Anna Wilde.

It is based on Jekyll and tailwindcss.

# Blog Posts

We've included support for DecapCMS for the blog posts.
This will allow you to create and edit blog posts locally using a browser. This means,
the browser will access you locally deployed website, and will create files locally
where this repository is. Then, using git, you can push your new files and changes as usual.
Because the website has separate DE and EN languages sites, you will need to add one post 
for each language.

To run the content management system (CMS), first deploy the website locally with the installation 
directions below. 

Then, run
```
npx decap-server
```

Go to the url [http://127.0.0.1:4000/admin](http://127.0.0.1:4000/admin)
This should automatically load the CMS, and you should see something like
![decap-screenshot](decap-screenshot.png)


# Installation

To develop and deploy the website locally, you will need to install ruby, and node.js. 

Then, run
```
npm install
bundle install
```

then you can run tailwind and have it auto update the styles.css file with
```
npm run build-css
```

and you can serve the website with
```
bundle exec jekyll serve
```
