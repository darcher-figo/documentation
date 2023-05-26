# <hr /> <sup>Title</sup> <img align="right" alt="IPG" src="./img/logo.svg" width="164" valign="middle" />

<a name="top"></a>

This `webview` encapsulates the payment form for users interacting with the quote flow and will be reused across `android`, `ios`, and `web`.

## <sup>Table of Contents</sup>

<table align="right">
<tr><th scope="col"><sub><sup>DOCUMENTATION</sup></sub></td></tr><tr><td><br />

<sup> &rsaquo; [<b>Code of Conduct</b>](.github/CODE_OF_CONDUCT.md)<br />
&rsaquo; [<b>Code Owners</b>](.github/CODEOWNER.md)<br />
&rsaquo; [<b>Contributing</b>](.github/CONTRIBUTING.md)<br />
&rsaquo; [<b>Guidelines</b>](.github/DEVELOPMENT.md)<br />
&rsaquo; [<b>Licensing</b>](LICENSE.md)<br />
</td></tr>
<tr><th scope="col"><sup><sub>TECHNOLOGY</sub></sup></th></tr><tr><td align="center"><br />

<img alt="React" src="https://cdn0.iconfinder.com/data/icons/logos-brands-in-colors/128/react_color-256.png" width="23"/><!--
--> <img alt="HTML5" src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/38/HTML5_Badge.svg/640px-HTML5_Badge.svg.png" width="23"/><!--
--> <img alt="Jest" src="https://cdn.auth0.com/blog/testing-react-with-jest/logo.png" width="21.5" /><!--
--> <img alt="ESLint" src="https://upload.wikimedia.org/wikipedia/commons/thumb/e/e3/ESLint_logo.svg/640px-ESLint_logo.svg.png" width="27" /><br /><!--
--> <img alt="Typescript" src="https://upload.wikimedia.org/wikipedia/commons/thumb/4/4c/Typescript_logo_2020.svg/640px-Typescript_logo_2020.svg.png" width="23" /><!--
--> <img alt="SASS" src="https://upload.wikimedia.org/wikipedia/commons/thumb/9/96/Sass_Logo_Color.svg/640px-Sass_Logo_Color.svg.png" width="29" /><!--
--> <img alt="NodeJS" src="https://upload.wikimedia.org/wikipedia/commons/thumb/d/d9/Node.js_logo.svg/640px-Node.js_logo.svg.png" width="40" ><!--
--> <img alt="Github" src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/3f/Git_icon.svg/640px-Git_icon.svg.png" width="22" /><!--
--> <br /><br /></td></tr>
<tr><th scope="col"><sup><sub>BADGES</sub></sup></td></tr>

<tr><td align="center"><br />

[![Issues][issues-shield]][issues-url]<br />
[![MIT License][license-shield]][license-url]<br />
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]<br />
[![Contributors][contributors-shield]][contributors-url]
<br /><br /></th></tr></table>

- [ Title ](#-title-)
  - [Table of Contents](#table-of-contents)
  - [Installation](#installation)
    - [ Clone project and go to directory](#-clone-project-and-go-to-directory)
    - [ Alignment to specified `node` version](#-alignment-to-specified-node-version)
    - [ Removes dynamicly generated directories](#-removes-dynamicly-generated-directories)
    - [ Install package dependencies](#-install-package-dependencies)
    - [ Launch `dev` instance to browser](#-launch-dev-instance-to-browser)
  - [Configuration](#configuration)
    - [ Artifactory](#-artifactory)
    - [ Environment variables `.env`](#-environment-variables-env)
  - [Maintinence](#maintinence)
    - [ Formats project code for readability and familiarity](#-formats-project-code-for-readability-and-familiarity)
  - [Linting](#linting)
    - [ Lints project code to reduce syntax errors](#-lints-project-code-to-reduce-syntax-errors)
  - [Testing](#testing)
    - [ Executes unit and e2e test suites to ensure quality](#-executes-unit-and-e2e-test-suites-to-ensure-quality)
    - [ Lints commit messages for a readable `git` history](#-lints-commit-messages-for-a-readable-git-history)
  - [Building](#building)
    - [ Bundle to `dist` folder](#-bundle-to-dist-folder)
    - [ Start production instance](#-start-production-instance)
  - [Versioning](#versioning)

---

## <sub>Installation</sub>

> **NOTE:** due to some dependency oddities, I swapped back to `yarn` for this project. You're able to use `npm` if you choose to; however, start the discussion prior to using a different package manager as there may be unanticipated ramifications by doing so.

### <sup> Clone project and go to directory</sup>

Setup usign `create-expo-app` and clear dependencies as well as references to `npm`.

> ```sh
> # or npx create-expo-app webview
> gh repo clone darcher-figo/webview
>
> # go to project
> cd webview
> ```

### <sup> Alignment to specified `node` version</sup>

> ```sh
> # using nvm
> nvm install v18.16.0
> nvm use
>
> # using npm
> npm install -g n
> sudo n stable # or 18.16.0
> ```

### <sup> Removes dynamicly generated directories</sup>

> ```sh
> yarn run clean
> ```

### <sup> Install package dependencies</sup>

> ```sh
> # install deps
> yarn
>
> # update deps if necessary
> yarn upgrade --latest
> ```

### <sup> Launch `dev` instance to browser</sup>

> ```sh
> # run dev in localhost instance
> yarn run web
>
> # additional options
> yarn run android
> yarn run ios
> yarn run start 
> ```

<table align="right"><tr><td>

<a href="#top" title="Return to top">:top:</a></td></tr></table>

## <sub>Configuration</sub>

Below is a configuration check to ensure each expected variable is defined and passed as a configuration export.

### <sup> Artifactory

> :soon: Include configurations to pull from *Artifactory*

### <sup> Environment variables `.env`</sup>

> :soon: Include `dotenv` to setup any global variables.

> ```txt
> PORT=3000
> HTTP=http
> HOST=localhost
>
> LOG_LVL=verbose
> ENABLE_LOGS=true
> NODE_ENV=development
> PUBLIC_URL=localhost:3000
> ```

## <sub>Maintinence</sub>

### <sup> Formats project code for readability and familiarity</sup>

> ```sh
> yarn run format
> ```

<table align="right"><tr><td>

<a href="#top" title="Return to top">:top:</a></td></tr></table>

## <sub>Linting</sub>

### <sup> Lints project code to reduce syntax errors</sup>

> ```sh
> yarn run lint
> ```

## <sub>Testing</sub>

### <sup> Executes unit and e2e test suites to ensure quality</sup>

> ```sh
> yarn run test # executes Jest & Playwright: e2e, indegration, & unit tests
> ```

### <sup> Lints commit messages for a readable `git` history</sup>

> ```sh
> yarn run lint:commit
> ```

<table align="right"><tr><td>

<a href="#top" title="Return to top">:top:</a></td></tr></table>

## <sub>Building</sub>

### <sup> Bundle to `dist` folder</sup>

> ```sh
> yarn run build
> ```

### <sup> Start production instance</sup>

> ```sh
> yarn start
> ```

## <sub>Versioning</sub>

> :soon: Implement [SemVer][sem-ver-url] for version automation.

<table align="right"><tr><td>

<a href="#top" title="Return to top">:top:</a></td></tr></table>

---

<br />
<table align="center"><tr><td valign="middle">

&copy; ммххɪɪɪ PetPartners, Inc.</td><td>
<a href="#top" title="Return to top">:top:</a></td></tr></table>

[js-api-url]: https://developer.mozilla.org/en-US/docs/Web/JavaScript
[web-components-url]: https://developer.mozilla.org/en-US/docs/Web/API/Web_components
[ipg-url]: https://www.independencepetgroup.com/
[sem-ver-url]: http://semver.org/
[contributors-shield]: https://img.shields.io/github/contributors/darcher-figo/webview.svg
[contributors-url]: https://github.com/darcher-figo/webview/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/darcher-figo/webview.svg
[forks-url]: https://github.com/darcher-figo/webview/network/members
[stars-shield]: https://img.shields.io/github/stars/darcher-figo/webview.svg
[stars-url]: https://github.com/darcher-figo/webview/stargazers
[issues-shield]: https://img.shields.io/github/issues/darcher-figo/webview.svg
[issues-url]: https://github.com/darcher-figo/webview/issues
[license-shield]: https://img.shields.io/github/license/darcher-figo/webview.svg
[license-url]: https://github.com/darcher-figo/webview/blob/master/LICENSE.txt