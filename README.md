# Tailwind Playground

A simple starter project for playing around with Tailwind CSS+UI in a proper PostCSS environment. This template also has an html include feature, so there aren't many duplicate templates.

## Getting Started

Clone the repository using this command:

   ```bash
   git clone https://github.com/lrfahmi/tailwind-playground.git tailwind-playground
   cd tailwind-playground
   ```

Then, install the dependencies:

   ```bash
   # Using npm
   npm install --also=dev

   # Using Yarn
   yarn
   ```

Finaly, Start the development server:

   ```bash
   # Using npm
   npm run serve

   # Using Yarn
   yarn serve
   ```

   Now you should be able to see the project running at localhost:8080.

## Crafting HTML
Create or open html files in `.html` folder in your editor to start experimenting. You don't need to change the html file that is in the `public` folder, it is generated automatically. Unless you want to add resources, such as js, img to a public folder.

### Include File
You can add an html file with content as below:

```
<!doctype html>
<html lang="en">
   <head>
      ${require('./_head.html')}
   </head>

...
```

## Building for production

Even though this isn't necessarily a starter kit for a proper project, we've included an example of setting up [cssnano](https://cssnano.co/) to optimize your CSS for production.
To build an optimized version of your CSS, simply run:

```bash
# Using npm
npm run production

# Using Yarn
yarn production
```

After that's done, check out `./public/build/tailwind.css` to see the optimized output.
