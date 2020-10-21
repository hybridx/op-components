# opc-timeline Component 👋

![Version](https://img.shields.io/badge/version-0.0.1-blue.svg?cacheSeconds=2592000)
![Build Status](https://travis-ci.org/dwyl/esta.svg?branch=master)
[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/1-Platform/op-components/graphs/commit-activity)

A web component based on Lit Element to show a timeline for a specific range

## Prerequisites
<!-- Add if any -->

## Usage
<!-- Add usage here -->

```html
<opc-timeline></opc-timeline>
```

## Slots
<!-- Add Slots here -->

## Attributes
<!-- Add attributes here -->

## Themes
<!-- Change colors here -->

| color   | hex                                                              |
|---------|------------------------------------------------------------------|
| --opc-timeline--BackgroundColor | <span class="readme-color-preview" style="--bg:#DEDEDE"></span> #DEDEDE |
| --opc-timeline--Color--step | <span class="readme-color-preview" style="--bg:#689B7A"></span> #689B7A |
| --opc-timeline--TextColor | <span class="readme-color-preview" style="--bg:#6C6C6C"></span> #6C6C6C |
| --opc-timeline--Color--active | <span class="readme-color-preview" style="--bg:#0aa521"></span> #0aa521 |
| --opc-timeline--Color--after-active | <span class="readme-color-preview" style="--bg:#b6e4bc"></span> #b6e4bc |

## Install

```sh
npm install
```

## Usage

### Install opc-timeline

```sh
npm install --save @one-platform/opc-timeline 
```

### For VanillaJS
- Import component
```js
import '@one-platform/opc-timeline';
```
- Add component in html
```html
<opc-timeline id="timeline1" current-step-index="1">
    <span slot="start-label" style="font-weight: 600;">Loaned on: Apr 28, 2018</span>
    <span slot="end-label" style="font-weight: 600;">Expires on: Oct 27, 2018</span>
</opc-timeline>
<script>
  document.querySelector('#timeline1').steps = [ 'Scheduled', 'Loaned', 'Extended', 'Completed'];
</script>
```

### For Angular
- In your app.module include the `CUSTOM_ELEMENTS_SCHEMA` and import the component
```js
import { NgModule, CUSTOM_ELEMENTS_SCHEMA } from '@angular/core';
import '@one-platform/opc-timeline';

@NgModule({
  declarations: [
    AppComponent,
  ],
  imports: [
    BrowserModule,
  ],
  schemas: [CUSTOM_ELEMENTS_SCHEMA],
  providers: [],
  bootstrap: [AppComponent]
})
export class AppModule { }
```
- Add component in any component html template
```html
<opc-timeline>
</opc-timeline>
```

### For React
- Import the component in App.js
```js
import '@one-platform/opc-timeline';
```

- Add component in any component html render
```html
<opc-timeline>
</opc-timeline>
```

### Development server

- Run development server

```sh
npm run dev opc-timeline
```

### Build

```sh
npm run build opc-timeline
```

## Run tests

```sh
npm run test
```

## 🤝 Contributors

👤 **hybridx**