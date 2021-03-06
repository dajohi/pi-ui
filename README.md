# pi-ui

> Politeia UI library
[documentation](https://compassionate-lalande-d3ef5d.netlify.com/)

[![NPM](https://img.shields.io/npm/v/pi-ui.svg)](https://www.npmjs.com/package/pi-ui) [![JavaScript Style Guide](https://img.shields.io/badge/code_style-standard-brightgreen.svg)](https://standardjs.com)

## Install

Make sure you have [nodejs](https://nodejs.org/en/) 8+ and [yarn](https://yarnpkg.com/en/) or [npm](https://www.npmjs.com/) installed.

#### yarn

```bash
yarn add pi-ui
```

#### npm

```bash
npm install --save pi-ui
```

## Usage

```jsx
import React, { Component } from "react";

import { Button } from "pi-ui";

class Example extends Component {
  render() {
    return <Button />;
  }
}
```

## Developing

- Clone this repository
- Install all deps by running:
  `yarn`
- If you're developing only on pi-ui, serving the live documentation should be enough:
  `yarn docz:dev`

- If you want to see your changes reflected in a project consuming pi-ui, you can use yarn link:
    - Go to the pi-ui directory on your machine and run:
    `yarn link`
    - Go to the project using pi-ui and run: 
    `yarn link pi-ui`

**Troubleshooting:**
 If you find some kind of incompatibility between react versions, link the react package from the main repository into pi-ui:
  
- Go to the main repository which is using the pi-ui lib, access the react folder inside its node_modules:
     - `cd /some/project/node_modules/react && yarn link`
     - `cd /pi-ui && yarn link react`
