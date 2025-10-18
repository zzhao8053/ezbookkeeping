# ezBookkeeping

[![License](https://img.shields.io/badge/license-MIT-green.svg)](https://github.com/zzhao8053/ezbookkeeping/blob/master/LICENSE)
[![Go Report](https://goreportcard.com/badge/github.com/zzhao8053/ezbookkeeping)](https://goreportcard.com/report/github.com/zzhao8053/ezbookkeeping)
[![Latest Release](https://img.shields.io/github/release/zzhao8053/ezbookkeeping.svg?style=flat)](https://github.com/zzhao8053/ezbookkeeping/releases)
[![Latest Build](https://img.shields.io/github/actions/workflow/status/zzhao8053/ezbookkeeping/build-snapshot.yml?branch=main)](https://github.com/zzhao8053/ezbookkeeping/actions)
[![Latest Docker Image Size](https://img.shields.io/docker/image-size/zzhao8053/ezbookkeeping.svg?style=flat)](https://hub.docker.com/r/zzhao8053/ezbookkeeping)
[![Docker Pulls](https://img.shields.io/docker/pulls/zzhao8053/ezbookkeeping)](https://hub.docker.com/r/zzhao8053/ezbookkeeping)
[![Ask DeepWiki](https://deepwiki.com/badge.svg)](https://deepwiki.com/zzhao8053/ezbookkeeping)

[![Recommend By HelloGitHub](https://api.hellogithub.com/v1/widgets/recommend.svg?rid=ded5af09da574ec1811ddb154f1b2093&claim_uid=LT7EZxeBukCnh0K)](https://hellogithub.com/en/repository/zzhao8053/ezbookkeeping)
[![Trending](https://trendshift.io/api/badge/repositories/12917)](https://trendshift.io/repositories/12917)

## Introduction

ezBookkeeping is a lightweight, self-hosted personal finance app with a user-friendly interface and powerful bookkeeping features. It's easy to deploy, and you can start it with just one single Docker command. Designed to be resource-efficient and highly scalable, it can run smoothly on devices as small as a Raspberry Pi, or scale up to NAS, MicroServers, and even large cluster environments.

ezBookkeeping offers tailored interfaces for both mobile and desktop devices. With support for PWA (Progressive Web Apps), you can even [add it to your mobile home screen](https://raw.githubusercontent.com/wiki/zzhao8053/ezbookkeeping/img/mobile/add_to_home_screen.gif) and use it like a native app.

Live Demo: [https://ezbookkeeping-demo.zzhao8053.net](https://ezbookkeeping-demo.zzhao8053.net)

## Features

-   **Open Source & Self-Hosted**
    -   Built for privacy and control
-   **Lightweight & Fast**
    -   Optimized for performance, runs smoothly even on low-resource environments
-   **Easy Installation**
    -   Docker-ready
    -   Supports SQLite, MySQL, PostgreSQL
    -   Cross-platform (Windows, macOS, Linux)
    -   Works on x86, amd64, ARM architectures
-   **User-Friendly Interface**
    -   UI optimized for both mobile and desktop
    -   PWA support for native-like mobile experience
    -   Dark mode
-   **AI-Powered Features**
    -   Receipt image recognition
    -   Supports MCP (Model Context Protocol) for AI integration
-   **Powerful Bookkeeping**
    -   Two-level accounts and categories
    -   Attach images to transactions
    -   Location tracking with maps
    -   Recurring transactions
    -   Advanced filtering, search, visualization, and analysis
-   **Localization & Globalization**
    -   Multi-language and multi-currency support
    -   Automatic exchange rates
    -   Multi-timezone awareness
    -   Custom formats for dates, numbers, and currencies
-   **Security**
    -   Two-factor authentication (2FA)
    -   Login rate limiting
    -   Application lock (PIN code / WebAuthn)
-   **Data Import/Export**
    -   Supports CSV, OFX, QFX, QIF, IIF, Camt.053, MT940, GnuCash, Firefly III, Beancount, and more

## Screenshots

### Desktop Version

[![ezBookkeeping](https://raw.githubusercontent.com/wiki/zzhao8053/ezbookkeeping/img/desktop/en.png)](https://raw.githubusercontent.com/wiki/zzhao8053/ezbookkeeping/img/desktop/en.png)

### Mobile Version

[![ezBookkeeping](https://raw.githubusercontent.com/wiki/zzhao8053/ezbookkeeping/img/mobile/en.png)](https://raw.githubusercontent.com/wiki/zzhao8053/ezbookkeeping/img/mobile/en.png)

## Installation

### Run with Docker

Visit [Docker Hub](https://hub.docker.com/r/zzhao8053/ezbookkeeping) to see all images and tags.

**Latest Release:**

    $ docker run -p8080:8080 zzhao8053/ezbookkeeping

**Latest Daily Build:**

    $ docker run -p8080:8080 zzhao8053/ezbookkeeping:latest-snapshot

### Install from Binary

Download the latest release: [https://github.com/zzhao8053/ezbookkeeping/releases](https://github.com/zzhao8053/ezbookkeeping/releases)

**Linux / macOS**

    $ ./ezbookkeeping server run

**Windows**

    > .\ezbookkeeping.exe server run

By default, ezBookkeeping listens on port 8080. You can then visit `http://{YOUR_HOST_ADDRESS}:8080/` .

### Build from Source

Make sure you have [Golang](https://golang.org/), [GCC](http://gcc.gnu.org/), [Node.js](https://nodejs.org/) and [NPM](https://www.npmjs.com/) installed. Then download the source code, and follow these steps:

**Linux / macOS**

    $ ./build.sh package -o ezbookkeeping.tar.gz

All the files will be packaged in `ezbookkeeping.tar.gz`.

**Windows**

    > .\build.bat package -o ezbookkeeping.zip

or

    PS > .\build.ps1 package -Output ezbookkeeping.zip

All the files will be packaged in `ezbookkeeping.zip`.

You can also build a Docker image. Make sure you have [Docker](https://www.docker.com/) installed, then follow these steps:

**Linux**

    $ ./build.sh docker

## Contributing

We welcome contributions of all kinds.

Found a bug? [Submit an issue](https://github.com/zzhao8053/ezbookkeeping/issues)

Want to contribute code? Feel free to fork and send a pull request.

Contributions of all kinds — bug reports, feature suggestions, documentation improvements, or code — are highly appreciated.

Check out our [Contributor Graph](https://github.com/zzhao8053/ezbookkeeping/graphs/contributors) to see the amazing people who've already helped.

## Translating

Help make ezBookkeeping accessible to users around the world. If you want to contribute a translation, please refer to our [translation guide](https://ezbookkeeping.zzhao8053.net/translating).

Currently available translations:

| Tag     | Language           | Contributors                                         |
| ------- | ------------------ | ---------------------------------------------------- |
| de      | Deutsch            | [@chrgm](https://github.com/chrgm)                   |
| en      | English            | /                                                    |
| es      | Español            | [@Miguelonlonlon](https://github.com/Miguelonlonlon) |
| fr      | Français           | [@brieucdlf](https://github.com/brieucdlf)           |
| it      | Italiano           | [@waron97](https://github.com/waron97)               |
| ja      | 日本語             | [@tkymmm](https://github.com/tkymmm)                 |
| ko      | 한국어             | [@overworks](https://github.com/overworks)           |
| nl      | Nederlands         | [@automagic](https://github.com/automagics)          |
| pt-BR   | Português (Brasil) | [@thecodergus](https://github.com/thecodergus)       |
| ru      | Русский            | [@artegoser](https://github.com/artegoser)           |
| th      | ไทย                | [@natthavat28](https://github.com/natthavat28)       |
| uk      | Українська         | [@nktlitvinenko](https://github.com/nktlitvinenko)   |
| vi      | Tiếng Việt         | [@f97](https://github.com/f97)                       |
| zh-Hans | 中文 (简体)        | /                                                    |
| zh-Hant | 中文 (繁體)        | /                                                    |

Don't see your language? Help us add it.

## Documentation

1. [English](http://ezbookkeeping.zzhao8053.net)
1. [中文 (简体)](http://ezbookkeeping.zzhao8053.net/zh_Hans)

## License

[MIT](https://github.com/zzhao8053/ezbookkeeping/blob/master/LICENSE)
