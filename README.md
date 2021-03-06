# Introduction

![Generator](https://github.com/merlinofcha0s/generator-jhipster-flutter/workflows/Generator/badge.svg?branch=master&event=push)
![npm version](https://img.shields.io/npm/v/generator-jhipster-flutter-merlin)

This is a [JHipster](https://www.jhipster.tech/) flutter blueprint.

# Prerequisites

As this is a [JHipster](https://www.jhipster.tech/) blueprint, we expect you have JHipster and its related tools already installed:

- [Installing JHipster (6.x.x)](https://www.jhipster.tech/installation/)
- [Installing Flutter SDK (1.17)](https://flutter.dev/docs/get-started/install)
- Generating server side with 

```bash
jhipster
```

# What's inside

- Main Screen
- Register
- Login
- I18n with EN and FR by default (WIP : need to add options to generate only desired languages)
- BLoC Architecture
- Android / iOS files by default (WIP : need to add options to generate only desired OS)
- Kotlin / Swift by default

# Installation

## With NPM

To install this blueprint:

```bash
npm install -g generator-jhipster-flutter-merlin
```

To update this blueprint:

```bash
npm update -g generator-jhipster-flutter-merlin
```

## With Yarn

To install this blueprint:

```bash
yarn global add generator-jhipster-flutter-merlin
```

To update this blueprint:

```bash
yarn global upgrade generator-jhipster-flutter-merlin
```

# Usage

To use this blueprint, run 

```bash
jhipster --blueprints flutter-merlin
```

# Architecture

For now the app is using BLoC pattern [More informations](https://medium.com/flutterpub/architecting-your-flutter-project-bd04e144a8f1)

## Main Libraries

- [dart_json_mapper](https://pub.dev/packages/dart_json_mapper)
- [flutter_intl](https://plugins.jetbrains.com/plugin/13666-flutter-intl)

## Running local Blueprint version for development

During development of blueprint, please note the below steps. They are very important.

1. Clone the projects

You'll probably need the current master of **generator-jhipster** :

- fork generator-jhipster: `https://github.com/jhipster/generator-jhipster/fork`
- clone locally your fork: `git clone https://github.com/<your_username>/generator-jhipster`
- `cd generator-jhipster`
- `git remote add upstream https://github.com/jhipster/generator-jhipster`
- so you'll be able to update regularly your fork, using `git fetch upstream && git checkout master && git rebase upstream/master`
- `npm ci`
- `npm link`

Then, about **jhipster-flutter** :

- fork jhipster-flutter: `https://github.com/jhipster/jhipster-flutter/fork`
- clone locally your fork: `git clone https://github.com/<your_username>/jhipster-flutter`
- `cd jhipster-flutter`
- `git remote add upstream https://github.com/jhipster/jhipster-flutter`
- so you'll be able to update regularly your fork, using `git fetch upstream && git checkout master && git rebase upstream/master`
- `npm ci`
- `npm link`
- `npm link generator-jhipster`


2. Create a new folder for the app to be generated and link JHipster and your blueprint there

```bash
mkdir my-app
cd my-app
npm link generator-jhipster-flutter-merlin
jhipster -d --blueprints flutter-merlin
```

# Help and contribution to the project

Feel free to help, the project is open to PR

# License

Apache-2.0 © Cyril Casaucau
