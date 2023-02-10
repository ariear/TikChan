[![npm version](https://badge.fury.io/js/tikchan.svg)](https://badge.fury.io/js/tikchan)

# TikChan

> a package that you can use to download video tiktok no watermark and more

## Table of contents

- [TikChan](#tikchan)
  - [Getting Started](#getting-started)
  - [Installation](#installation)
  - [Usage](#usage)
  - [API](#api)
    - [download](#download)
  - [Versioning](#versioning)
  - [Authors](#authors)

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

## Installation

Start with install library using yarn or npm:

```sh
$ npm install tikchan
```

Or if you prefer using Yarn:

```sh
$ yarn add tikchan
```

```js
 const TikChan = require('mengscrape-manga')
```

## Usage

Scripts

```js
 TikChan.download('https://www.tiktok.com/@gelap106/video/7160002182283054363?is_from_webapp=1&sender_device=pc&web_id=7196247961113200130').then(results => {
    console.log(results);
  }).catch(err => {
    console.log(err);    
  })
```
If you using asynchronous 
```js
  async function DownloadTest(url) {
    const results = await TikChan.download(url)
    console.log(results);
  }
```

Output
```js
{
  no_wm: 'https://ttdownloader.com/dl.php?v=YTo0OntzOjk6IndhdGVybWFyayI7YjowO3M6NzoidmlkZW9JZCI7czozMjoiYTdlMWY0YjBjNjg0YzQxMWNlNTc1YjViZmY2NzFkNTkiO3M6MzoidWlkIjtzOjMyOiIxODlhMWIyNTRmNDhkNzkwY2U2NzE1NTBmZTk1ZThlZCI7czo0OiJ0aW1lIjtpOjE2NzYwMzI4ODE7fQ==',
  wm: 'https://ttdownloader.com/dl.php?v=YTo0OntzOjk6IndhdGVybWFyayI7YjoxO3M6NzoidmlkZW9JZCI7czozMjoiYTdlMWY0YjBjNjg0YzQxMWNlNTc1YjViZmY2NzFkNTkiO3M6MzoidWlkIjtzOjMyOiIxODlhMWIyNTRmNDhkNzkwY2U2NzE1NTBmZTk1ZThlZCI7czo0OiJ0aW1lIjtpOjE2NzYwMzI4ODE7fQ=='
}
```

## API

### Download

```js
TikChan.download(url)
```

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/ariear/TikChan/tags).

## Authors

* **Arie Akbarull Ridho** - *ariear* - [ariear](https://github.com/ariear)

See also the list of [contributors](https://github.com/ariear/TikChan/contributors) who participated in this project.

