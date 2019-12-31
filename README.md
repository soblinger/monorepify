[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]


<br />
<p align="center">
  <a href="#">
    <img src="readme-images/logo.png" alt="monorepify-logo" width="80" height="80">
  </a>

  <h3 align="center">Monorepify</h3>

  <p align="center">
    A boilerplate for Full stack VueJS and nestJS and other typescript frameworks too. But i believe you can add JS frameworks too (with little modification)
    <br />
    <br />
    <a href="https://github.com/emjimadhu/monorepify/issues">Report Bug</a>
    ·
    <a href="https://github.com/emjimadhu/monorepify/issues">Request Feature</a>
  </p>
</p>



## Table of Contents

* [About the Project](#about-the-project)
  * [Built With](#built-with)
* [Getting Started](#getting-started)
  * [Prerequisites](#prerequisites)
  * [Installation](#installation)
* [Scripts](#scripts)
* [License](#license)
* [Contact](#contact)



## About The Project

[![Monorepify Screen Shot][product-screenshot]](#)

I like monorepos for code sharing between multiple projects in a single codebase. For other frameworks like angular, react, nest, express, There is wonderful tool called **NX**. They don't support Vue (for now). That's why i created this boilerplate. But you can you any JS Frameworks with little tweaks!

A list of commonly used resources that I find helpful are listed in the acknowledgements.

### Built With
* [NodeJS](https://nodejs.org)
* [Yarn](https://yarnpkg.com)
* [Vue](https://vuejs.org)
* [NestJS](https://nestjs.com/)

## Getting Started

### Required Versions

- **node** - v12.13.1
- **npm** - v6.12.1
- **yarn** - v1.21.1
- **vue** - v4.1.1
- **nest** - v6.5.9 

### Prerequisites

Tools and Services need to run this app.

* node
```sh
# Mac and Linux using nvm (node-version-manager)
curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.33.0/install.sh | bash

nvm install v12.13.1
```

* yarn
```sh
# Mac
brew install yarn

# Debian / Ubuntu
curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | sudo apt-key add -
echo "deb https://dl.yarnpkg.com/debian/ stable main" | sudo tee /etc/apt/sources.list.d/yarn.list
sudo apt update && sudo apt install yarn
```

* nestjs
```sh
# Mac and Linux using nvm (node-version-manager)
npm i -g @nestjs/cli
```

### Installation

1. Clone the repo
```sh
git clone #
```
2. Install NPM packages
```sh
yarn install
```

## Scripts

* `yarn run dev:all:start` - Starts Development server for shared, client and server,
* `yarn run dev:all:build` - Builds shared, client and server,
* `yarn run dev:client:start` - Starts client development server,
* `yarn run dev:client:build` - Builds client,
* `yarn run dev:client:lint` - Lints client,
* `yarn run test:client:unit` - Unit testing for client,
* `yarn run test:client:e2e` - End to End testing for client,
* `yarn run dev:server:start` - Starts server development server,
* `yarn run dev:server:build` - Builds server,
* `yarn run dev:server:lint` - Lints server,
* `yarn run prod:server:start` - Starts server in production mode,
* `yarn run dev:shared:start` - Starts shared development server,
* `yarn run dev:shared:build` - Builds shared,
* `yarn run dev-shared:client:start` - Starts shared and client in development mode,
* `yarn run dev-shared:server:start` - Starts shared and server in development mode,
* `yarn run dev-shared:client:build` - Builds shared and client,
* `yarn run dev-shared:server:build` - Builds shared and server,
* `yarn run utils:remove-node-modules` - Removes all node_modules folders

## Directory Structure

- `root`: Project root holds all the fies of the project
    - `apps`: Holds client(VueJS) and server(NestJS) projects (You can add any client or server frameworks in here in addition or replace with existing ones. See section `Add other frameworks` in `How To`)
        - `client`: A Vue project created using vue-cli
        - `server`: A Nest project created using nest-cli
    - `libs`: Holds all the common codes you can share between projects
        - `shared`: A shared module for common code sharing across projects in this work space.
    - `readme-images`: Holds all the images for README.

## How to

- ### Code Scaffolding
    - #### Client (VueJS)
        - `cd apps/client`
        - `# Run any vue-cli commands in here`
     - #### Server (NestJS)
       - `cd apps/server`
       - `# Run any nest-cli commands in here ex: nest g m <module-name>`
     - #### Shared (Typescript)
       - `cd libs/shared`
       - `# Creae any number of codes that you want to share and make sure you export the files in index.ts`
- ### Add other frameworks
    - ### Angular (Example)
        - `cd apps`
        - `ng new <app_name>`
        - Remove `node_modules` and `.gitigonre` in `<app_name>`
        - `tsconfig.json`: Put `../../tsconfig` in `extends` field of `tsconfig` and remove common tsconfig options which can be shared across projects.
        - Run `cd <root_directory> && yarn utils:remove-node-modules && yarn install`
     - I believe you can add other typescript frameworks with this same steps! (You can even add native JS frameworks with little of tweaking)

## License

Distributed under the MIT License. See `LICENSE` for more information.

## Contact

Em Ji Madhu - [Linkedin](https://www.linkedin.com/in/em-ji-madhu-8b007456/)

Project Link: [Monorepify](https://github.com/emjimadhu/monorepify)

[contributors-shield]: https://img.shields.io/github/contributors/othneildrew/Best-README-Template.svg?style=flat-square
[contributors-url]: https://github.com/emjimadhu/monorepify/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/othneildrew/Best-README-Template.svg?style=flat-square
[forks-url]: https://github.com/emjimadhu/monorepify/network/members
[stars-shield]: https://img.shields.io/github/stars/othneildrew/Best-README-Template.svg?style=flat-square
[stars-url]: https://github.com/emjimadhu/monorepify/stargazers
[issues-shield]: https://img.shields.io/github/issues/othneildrew/Best-README-Template.svg?style=flat-square
[issues-url]: https://github.com/emjimadhu/monorepify/issues
[license-shield]: https://img.shields.io/github/license/othneildrew/Best-README-Template.svg?style=flat-square
[license-url]: https://github.com/emjimadhu/monorepify/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=flat-square&logo=linkedin&colorB=1
[linkedin-url]: https://linkedin.com/in/othneildrew
[product-screenshot]: readme-images/screenshot.png