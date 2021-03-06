# Skeleton React Native

This repository contains a React Native App skeleton powered by React Native.

This repo has been built and tested using the following software and associated
versions, please ensure you meet the minimum version shown below for each in
order for this repo to run correctly.

![react native v0.45.1+](https://img.shields.io/badge/react_native-v0.45.1%2B-brightgreen.svg) ![react native cli v2.0.1+](https://img.shields.io/badge/react_native_cli-v2.0.1%2B-brightgreen.svg) ![node v8.1.3+](https://img.shields.io/badge/node-v8.1.3%2B-brightgreen.svg) ![npm v5.0.4+](https://img.shields.io/badge/npm-v5.0.4%2B-brightgreen.svg) ![homebrew v1.2.4+](https://img.shields.io/badge/homebrew-v1.2.4%2B-brightgreen.svg) ![watchman v4.7.0+](https://img.shields.io/badge/watchman-v4.7.0%2B-brightgreen.svg)


## Prerequisites

Before you clone this repository, please ensure the following 5 packages have been installed
<b>(first-time setup only)</b>. Please also ensure that you have node/NPM installed.
We are also using NPM to manage our project dependencies.

### Environment Setup

#### 1. Install XCode

Download it from Apple Store

#### 2. Install HomeBrew

```TXT
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```
Mac OSX dependencies management program used here to install node

#### 3. Install Node/NPM

```TXT
brew install node
```  
or if it's already installed

```TXT
brew upgrade node
```

Node runs Javascript outside of the browser.<br>
NPM is used for installing dependencies.<br>
Node and NPM come together, they are installed at the same time.

#### 4. Install Watchman

```TXT
brew install watchman
```

Watch filers on the hard drive and waits for them to change

#### 5. Install React Native CLI<br>

```TXT
npm install -g react-native-cli
```

Used to generate new React Native projects

# Let's get started

## Clone the repository

CD into your 'projects' folder and clone the repo with the git clone command.

```TXT
git clone git@github.com:frankdarnese/react-native-skeleton.git
```

## Update folder name && cd into it

Change the repository name according to your new project. Linux and Unix users
can rename their files and directories by using the
<a href="https://www.computerhope.com/unix/umv.htm">mv command</a>.<br>

```TXT
mv react-native-skeleton your_new_project_name && cd your_new_project_name
```

<b>Please note:</b> You can also rename the folder at the time you clone it.
See example below:

```TXT
git clone git@github.com:frankdarnese/react-native-skeleton.git YOUR_NEW_PROJECT_NAME && cd YOUR_NEW_PROJECT_NAME
```

## Install NPM

Run `npm install` within the project folder

## Build and run the project

To build and launch the project, run the following command:

- Option 1.<br>

```TXT
react-native run-ios
```

<b>Note</b>: This may take a few minutes before building the app. Once done, this
should launch the Simulator and you should see the boilerplate welcome screen.<br>

- Option 2.<br>

Start the app from the <a href="https://developer.apple.com/xcode/">Xcode IDE</a>

## Initializing GIT + GitHub remote setup

cd into the project folder and run

```TXT
  git init
  git commit -m "Initial commit"
  git remote add origin git@github.com:YOUR-REPOSITORY-NAME.git
  git push -u origin master
```

## Open the project folder in your favorite editor

e.g. If you are using atom:

```TXT
  atom react-native-skeleton
```
or if you are in the project folder already:

```TXT
  atom .
```

## Setup ES6 + Babel + JSX Linting with Atom (Optional)

This sets up Atom to properly lint ES6+Babel+JSX using Airbnb's .eslintrc as a
starting point.

1. In Atom install <b>lint & es-lint</b> packages

2. Install <b>eslint-config-airbnb babel-eslint eslint-plugin-react</b> which
are files that contains a set of rules we are going to use during our project.

From your project root run:

```TXT
npm install --save-dev eslint-config-airbnb babel-eslint eslint-plugin-react
```


3. Make sure ESLint knows to use the rule set-up/bundle we have just installed via NPM
Inside of the project directory create a new file called <b>.eslintrc</b>

4. Add the following code to the .eslintrc file
```TXT
  {
    "extends": "eslint-config-airbnb"
  }
```

Please check <a href="https://github.com/airbnb/javascript" target="blank">Airbnb's
Javascript styleguide</a> and the <a href="http://eslint.org/docs/user-guide/configuring#extending-configuration-files" target="blank">ESlint config docs</a> for more information.

## Testing

- To test the project inside the Simulator you can open the inspector mode
from within the Simulator menu (`CMD + D to show the menu`).

- For web testing/debugging you can go to : `http://localhost:8081/debugger-ui`
and open the web inspector.

- You may also install the <a href="https://github.com/facebook/react-devtools/tree/master/packages/react-devtools">standalone version of React Developer Tools</a> to inspect the React component hierarchy, their props, and state.<br>
When react-devtools is running, Inspector will enter a special collapsed mode,
and instead use the DevTools as primary UI. In this mode, clicking on something
in the simulator will bring up the relevant components in the DevTools.
Please check the <a href="https://github.com/facebook/react-devtools/tree/master/packages/react-devtools">React Developer Tools</a> on GITHUB for more info.
