# Angular Tutorial: Learn Angular from Scratch Step by Step

An Angular 7 + Angular Material front-end built while following the ["Learn Angular from scratch step by step"](https://angular-templates.io/tutorials/about/learn-angular-from-scratch-step-by-step) tutorial. Pairs with [learn-how-to-build-a-mean-stack-application](https://github.com/KewaneeMcGhee-Wiggins/learn-how-to-build-a-mean-stack-application) as the backend (LoopBack + MongoDB) REST API.

## Tech stack

- Angular 7, Angular Material, Angular CDK
- Bootstrap (Sass), Font Awesome

## Installation

```bash
npm install
ng serve
```

Then navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

### Building on a modern Node version

This is an Angular 7 project (webpack 4 under the hood), so building it with a current Node.js runtime hits two well-known issues:

1. **OpenSSL 3 / "digital envelope routines::unsupported"** — fixed by running with the legacy OpenSSL provider:
   ```bash
   NODE_OPTIONS=--openssl-legacy-provider ng build
   ```
2. **`node-sass` fails to load** — `node-sass` 4.x has no prebuilt binary for modern Node versions. The simplest fix is swapping it for `sass` (dart-sass), which is a drop-in replacement for the CLI's Sass compilation.

The easiest way to avoid both is to build/run this with Node 10 or 12, which is what the project originally targeted.

![](https://s3-us-west-2.amazonaws.com/angular-templates/tutorials/learn-angular-from-scratch-step-by-step/learn-angular-from-scratch-step-by-step-categories.png)
