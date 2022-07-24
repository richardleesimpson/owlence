# owlence

An app that makes it easy for owls to manage allowance for their owlet(s).

## The problem

My wife and I want to teach our children about managing money in the modern age. Simple, right?

Let's look at a couple of potential solutions and examine why they didn't fit our use case.

### Banks

The first thing you'd think to try; the old standard.
* The kids are still quite young, so we can't open bank accounts for them.
* Even if we could, [banks take advantage of you](https://www.debt.org/faqs/banks-take-advantage-of-you/). I don't want to support that business model any more than is strictly necessary.

### Cash

The next easiest way to take care of it, or so we thought.
* Who carries cash? We'd literally have to go out of town regularly just to get it.
* It gets damaged or lost, despite our best efforts to provide piggy banks and wallets.
* [Moonjars](https://moonjar.com) just don't hold a lot of bills, which is a problem when some kids get allowance in the single digits.

### Apps

Surely somebody has thought of this before!
* [They have](https://www.parents.com/kids/responsibility/money-management/allowance-and-budgeting-apps-for-kids), with varying features from service to service.
* Of all the options, I think [FamZoo](https://famzoo.com) is probably the most robust, but it [does have some drawbacks](https://wellkeptwallet.com/famzoo-review#Positives_and_Negatives).

I think we can make an app that takes the best features of all of these, improves on them a little, and avoids the pitfalls. Shall we? 

## Features
* coming soon! See below ;)

## The future

Good things are coming your way.
* accounts for owls, because we need to start somewhere
* linked accounts, for access to funds
* nests, for adding owlets and other owls
* nest keys, for interacting with the legacy banks
* manual owlence, for sending money to your owlets
* automatic owlence, for hands off savings
* jars, for splitting it up whatever way makes sense to you
* interest, for putting your money to work
* accounts for owlets, for when they have their own devices
* reports for owls, for when deviceless owlets want to know
* in-nest borrowing, for when your owlet simply cannot wait
* out-of-nest borrowing, for when *you* simply cannot wait
* cards, for letting them spend without needing you to get involved
* notifications, for the occasional helpful reminder

... and probably more over time!

## Getting started

Once you clone the repo and make sure you have [a few prerequisites installed](https://yarnpkg.com/getting-started/install), it's as simple as running a few commands in the root of the project:
```
yarn
yarn start
```
... and that's it. Have fun!

## Contributing

Have an idea for a good feature for the app? Want to get involved? [Email me!](mailto:richardleesimpson@pm.me)

## An ignited app!

[![CircleCI](https://circleci.com/gh/infinitered/ignite.svg?style=svg)](https://circleci.com/gh/infinitered/ignite)

### The latest and greatest boilerplate for Infinite Red opinions

This is the boilerplate that [Infinite Red](https://infinite.red) uses as a way to test bleeding-edge changes to our React Native stack.

Currently includes:

- React Native
- React Navigation
- MobX State Tree
- TypeScript
- And more!

### Quick Start

The Ignite boilerplate project's structure will look similar to this:

```
ignite-project
├── app
│   ├── components
│   ├── i18n
│   ├── utils
│   ├── models
│   ├── navigators
│   ├── screens
│   ├── services
│   ├── theme
│   ├── app.tsx
├── storybook
│   ├── views
│   ├── index.ts
│   ├── storybook-registry.ts
│   ├── storybook.ts
│   ├── toggle-storybook.tsx
├── test
│   ├── __snapshots__
│   ├── storyshots.test.ts.snap
│   ├── mock-i18n.ts
│   ├── mock-reactotron.ts
│   ├── setup.ts
│   ├── storyshots.test.ts
├── README.md
├── android
│   ├── app
│   ├── build.gradle
│   ├── gradle
│   ├── gradle.properties
│   ├── gradlew
│   ├── gradlew.bat
│   ├── keystores
│   └── settings.gradle
├── ignite
│   ├── ignite.json
│   └── plugins
├── index.js
├── ios
│   ├── IgniteProject
│   ├── IgniteProject-tvOS
│   ├── IgniteProject-tvOSTests
│   ├── IgniteProject.xcodeproj
│   └── IgniteProjectTests
├── .env
└── package.json

```

#### ./app directory

Included in an Ignite boilerplate project is the `app` directory. This is a directory you would normally have to create when using vanilla React Native.

The inside of the src directory looks similar to the following:

```
app
│── components
│── i18n
├── models
├── navigators
├── screens
├── services
├── theme
├── utils
└── app.tsx
```

**components**
This is where your React components will live. Each component will have a directory containing the `.tsx` file, along with a story file, and optionally `.presets`, and `.props` files for larger components. The app will come with some commonly used components like Button.

**i18n**
This is where your translations will live if you are using `react-native-i18n`.

**models**
This is where your app's models will live. Each model has a directory which will contain the `mobx-state-tree` model file, test file, and any other supporting files like actions, types, etc.

**navigators**
This is where your `react-navigation` navigators will live.

**screens**
This is where your screen components will live. A screen is a React component which will take up the entire screen and be part of the navigation hierarchy. Each screen will have a directory containing the `.tsx` file, along with any assets or other helper files.

**services**
Any services that interface with the outside world will live here (think REST APIs, Push Notifications, etc.).

**theme**
Here lives the theme for your application, including spacing, colors, and typography.

**utils**
This is a great place to put miscellaneous helpers and utilities. Things like date helpers, formatters, etc. are often found here. However, it should only be used for things that are truely shared across your application. If a helper or utility is only used by a specific component or model, consider co-locating your helper with that component or model.

**app.tsx** This is the entry point to your app. This is where you will find the main App component which renders the rest of the application.

#### ./ignite directory

The `ignite` directory stores all things Ignite, including CLI and boilerplate items. Here you will find generators, plugins and examples to help you get started with React Native.

#### ./storybook directory

This is where your stories will be registered and where the Storybook configs will live.

#### ./test directory

This directory will hold your Jest configs and mocks, as well as your [storyshots](https://github.com/storybooks/storybook/tree/master/addons/storyshots) test file. This is a file that contains the snapshots of all your component storybooks.

### Running Storybook

From the command line in your generated app's root directory, enter `yarn run storybook`
This starts up the storybook server and opens a story navigator in your browser. With your app
running, choose Toggle Storybook from the developer menu to switch to Storybook; you can then
use the story navigator in your browser to change stories.

For Visual Studio Code users, there is a handy extension that makes it easy to load Storybook use cases into a running emulator via tapping on items in the editor sidebar. Install the `React Native Storybook` extension by `Orta`, hit `cmd + shift + P` and select "Reconnect Storybook to VSCode". Expand the STORYBOOK section in the sidebar to see all use cases for components that have `.story.tsx` files in their directories.

### Running e2e tests

Read [e2e setup instructions](./e2e/README.md).

## License

This project is licensed under the GPL-3.0 license. [Read it here](./LICENSE).