<br/>
<p align="center">
  <a href="https://github.com/uiedbook/Naxtjs">
    <img src="naxt.png" alt="Logo" width="80" height="80">
  </a>

  <h1 align="center">Naxt</h1>

  <p align="center">
  Naxt - SSR library for server-side javascript 
    <br/>
    <br/>
    <a href="https://github.com/uiedbook/Naxtjs#examples"><strong>Explore the 🎙️ docs »</strong></a>
    <br/>
    <br/>
    <a href="https://t.me/UiedbookHQ">Join Community</a>
    .
    <a href="https://github.com/uiedbook/Naxtjs/issues">Report Bug</a>
    .
    <a href="https://github.com/uiedbook/Naxtjs/issues">Request Feature</a>
  </p>
</p>

![Contributors](https://img.shields.io/github/contributors/Uiedbook/Naxtjs?color=dark-green) ![Issues](https://img.shields.io/github/issues/Uiedbook/Naxtjs) ![License](https://img.shields.io/github/license/Uiedbook/Naxtjs)
[![npm Version](https://img.shields.io/npm/v/naxtjs.svg)](https://www.npmjs.com/package/Naxtjs)[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/uiedbook/Naxt.js/blob/next/contributing.md)![Forks](https://img.shields.io/github/forks/uiedbook/Naxtjs?style=social) ![Stargazers](https://img.shields.io/github/stars/uiedbook/naxtjs?style=social)

# Contents

- [What is Naxtjs](#what-is-Naxtjs)
- [Installation](#installation)
- [Examples](#example)
- [Getting Help](#getting-help)

## What is Naxtjs?

Naxt is a library framework for server side rendering.

Naxt is fast, and performant and is just 5KB.

Unlike htmx and qwirk, naxt only add 900 bytes of javascript to hydrate the dom and handle reactivity.

This makes naxt very efficient.

Naxt follows the [VJS specification](https://github.com/Uiedbook/cradova/blob/main/VJS_spec)

Please naxt work exactly like htmx but this docs is not complete to demostrate it yet.

If you want quick info check out our telegram group.

## Installation

### npm

```bash
npm i naxtjs
```

## Examples

Many aspects of Naxt are not reflected in the following example. More functionality will be entailed in future docs.

## A basic component in Naxtjs:

```js
import { div, h1, compile } from "naxtjs";

function Hello(name) {
  return h1("Hello " + name, {
    className: "title",
    style: {
      color: "grey",
    },
  });
}

const html = await compile("index.html", div(Hello("peter"), Hello("joe"))); // html string

app.get("/", (req, res) => {
  res.send(html);
});
```

## Getting Help and Contributing

To get further insights and help on Naxtjs, join [Telegram](https://t.me/uiedbookHQ) Community.
