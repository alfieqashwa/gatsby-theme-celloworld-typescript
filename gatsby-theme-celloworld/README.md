# The smallest possible Gatsby theme

## Quick Start

```shell
mkdir my-site
cd my-site
yarn init
# install gatsby-theme-celloworld and it's dependencies
yarn add gatsby react react-dom gatsby-theme-celloworld
```

Then add the theme to your `gatsby-config.js`. We'll use the long form
here for education purposes.

```javascript
module.exports = {
  plugins: [
    {
      resolve: "gatsby-theme-celloworld",
      options: {},
    },
  ],
}
```

That's it, you can now run your gatsby site using

```shell
yarn gatsby dev
```

Note that this site doesn't _do_ anything, so you're see a missing
resources error. Create a simple page in `src/pages/index.js` to see a
page on the root url.

```javascript
import React from "react"

export default () => <div>Cello, World!</div>
```

## Doing more with themes

You can use this as a place to start when developing themes. I
generally suggest using [yarn
workspaces](https://yarnpkg.com/lang/en/docs/workspaces/) like the
[gatsby-theme-examples repo
does](https://github.com/ChristopherBiscardi/gatsby-theme-examples),
but using `yarn link` or `npm link` is a viable alternative if you're
not familiar with workspaces.
