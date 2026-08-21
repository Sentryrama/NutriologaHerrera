# Nutriologa Herrera Landing Page

A simple single-page web application built with HTML, CSS, and JavaScript.

## Features

- Fast and lightweight
- Single-page client-side navigation


### Prerequisites

Make sure you have [Node.js](https://nodejs.org/) and [pnpm](https://pnpm.io/) installed.


### Add server with autoreload

*Option 1: [servor](https://npmx.dev/package/servor) (✅fast, ✅lightweight, ✅no dependencies)*

```bash
pnpm add servor
```
```bash
pnpx servor src/ index.html 1234 --reload
```

*Option 2: [live-server](https://npmx.dev/package/live-server)*

```bash
pnpm add live-sever
```
```bash
pnpx live-server src/ --no-browser --port=1234
```

*Option 3: [vite](https://npmx.dev/package/vite)*

```bash
pnpm add vite
```
```bash
pnpx vite src/ --port 1234
```