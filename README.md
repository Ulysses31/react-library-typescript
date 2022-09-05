# React Library using Typescript

## tutorial
```bash
https://dev.to/alexeagleson/how-to-create-and-publish-a-react-component-library-2oe
```

## Publishing your library
```bash
  In package.json insert ...

  {
  "name": "@YOUR_GITHUB_USERNAME/YOUR_REPOSITORY_NAME",
  "publishConfig": {
    "registry": "https://npm.pkg.github.com/YOUR_GITHUB_USERNAME"
  },
  ...  
}

```

```bash
Insert in ~/.npmrc the following content...

registry=https://registry.npmjs.org/
@YOUR_GITHUB_USERNAME:registry=https://npm.pkg.github.com/
//npm.pkg.github.com/:_authToken=YOUR_AUTH_TOKEN

```

```bash
And last run npm publish
```