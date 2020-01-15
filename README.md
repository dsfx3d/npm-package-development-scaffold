# npm-package-development-scaffold

> woosh...

A boilerplate project so you won't have to worry about the tedious task of setting up the local development environment for your next awesome npm package.

This got you covered from linting your code to automatic release on npm via CI.

## Installation

You can fork it :fork_and_knife: or clone it :sheep: and make it your own.

Or copy this repository in your system using [degit](https://www.npmjs.com/package/degit):


```bash
npx degit dsfx3d/npm-package-development-scaffold
```

## Setup

In a few steps, you can start building npm package:

> If you've copied the repository using degit, push an initial commit to github before you begin.

1. Login to [Travis](https://travis-ci.org/) using your GitHub account.

2. Create an account on [NPM](https://www.npmjs.com/package/degit). If you already have an account skip this step.

3. Install project dependencies:
   ```bash
   npm install
   ```
4. setup semantic-release
   ```bash
   npm run setup:release
   ```
   **Important:** Always use commit script to commit your work. Otherwise, the automatic release won't be triggered when you push to Github.
   ```bash
   npm run commit
   ```

5. And you're ready to develop :muscle:. You can now commit and push to GitHub. On every feature, fix and breaking commit your package will be released on noth GitHub and NPM. You don't have to worry about the

## What's included?

### Typescript

[Typescript](https://www.typescriptlang.org/) is a language of choice of many developers when developing npm packages. If you are not using it in your npm packages yet, you should.

### Prettier + tslint

[Prettier](https://www.npmjs.com/package/prettier), for code formatting. Formats not just javascript and typescript but a lot of other languages and not just programming languages but JSON, CSS, SCSS, HTML, Vue, Angular, GraphQL, Markdown, YAML etc. (**note:** A prettier plugin for your code editor is a recommended for better experience).

For everything else required for linting your code, there's always [tslint](https://palantir.github.io/tslint/).

### Jest

[Jest](https://jestjs.io/en/) is a delightful JavaScript Testing Framework with a focus on simplicity. Jest is a lot more than a test runner, it includes a powerful assertion library and code coverage reports. Go check docs.

### Babel

[Babel](https://babeljs.io/) is an OG when it comes to transpilers. If you are wondering why are we using babel if we already have typescript, you might wanna read this post. [TypeScript With Babel: A Beautiful Marriage](https://iamturns.com/typescript-babel/).

### Travis CI

[Travis CI](https://travis-ci.org/) is a hosted continuous integration service used to build and test software projects hosted at GitHub. Travis CI provides various paid plans for private projects and :sparkles: **a free plan for open source** :sparkles:.

Travis will test and release your package on NPM whenever you make a master commit on GitHub. You ask how? the next pointer is for you.

### Sementic Release CLI

> Trust us, this will change your workflow for the better. – egghead.io

[semantic-release](https://github.com/semantic-release/semantic-release) automates the whole package release workflow including: determining the next version number, generating the release notes and publishing the package.

This removes the immediate connection between human emotions and version numbers, strictly following the Semantic Versioning specification.

### Webpack (bonus)

If you wanna bundle your package for browsers, you can do that.

## Scripts

### Linting

   ```bash
   npm run lint
   npm run lint:fix
   ```

### Test

```bash
npm run test
```

### Build Package

```bash
npm run build
```

### Bundle package build

```bash
npm run bundle
```

### Commit

```bash
npm run commit
```


## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update the tests as appropriate.

## License
[MIT](https://choosealicense.com/licenses/mit/)
