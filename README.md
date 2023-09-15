# Creation UI

is a design system that lets you build a React powered websites
and apps. It's built on top of [Tailwind CSS](https://tailwindcss.com) and currently supports <b>React</b> and <b>Solid</b>.

A great starting point for your next project.

<br />

## Prerequisites

Creation UI is working with your app's Tailwind CSS and you need to have Tailwind CSS installed in your project - [Tailwind CSS Installation](https://tailwindcss.com/docs/installation/using-postcss).

```
  "peerDependencies": {
    "tailwindcss": "^3.0"
  },
```

## Installation

To install the core packages of Creation UI, run command below:

> yarn add @creation-ui/core

> npm i @creation-ui/core

> pnpm i @creation-ui/core



## Configuration

1. Add `withTailwindConfig` to your `tailwind.config.js` file:

```js copy
const withTailwindConfig = require('@creation-ui/react/utils/withTailwindConfig')

module.exports = withTailwindConfig({
  content: ['./**/*.{js,ts,jsx,tsx,mdx}', '*.css'],
})
```

You can extend all properties [as usual](https://tailwindcss.com/docs/configuration).

2. Import library's CSS file into your app.
   If you're using standard config of `Next.js`, you should import it in `pages/_app.js` or similar.
   If you're using standard config of `create-react-app` or `Vite`, you should import it in `index.js` or similar.

```js copy
import '@creation-ui/core/index.css'
```

3. Start using it!

If you are using either React or Solid you can add components by installing their respective packages:

### React
> yarn add @creation-ui/react

> npm i @creation-ui/react

> pnpm i @creation-ui/react

```jsx copy
import { Button } from '@creation-ui/react'

export default function App() {
  return <Button>Click me</Button>
}
```



### Solid
> yarn add @creation-ui/solid

> npm i @creation-ui/solid

> pnpm i @creation-ui/solid


```jsx copy
import { Button } from '@creation-ui/solid'

export default function App() {
  return <Button>Click me</Button>
}
```
