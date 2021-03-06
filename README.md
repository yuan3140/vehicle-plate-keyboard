# vehicle-plate-keyboard

[![npm version](https://badge.fury.io/js/vehicle-plate-keyboard.svg)](//npmjs.com/package/vehicle-plate-keyboard) [![Build Status](https://travis-ci.com/LiuuY/vehicle-plate-keyboard.svg?branch=master)](https://travis-ci.com/LiuuY/vehicle-plate-keyboard) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![Storybook](https://cdn.jsdelivr.net/gh/storybookjs/brand@master/badge/badge-storybook.svg)](https://github.com/LiuuY/vehicle-plate-keyboard)

A Chinese vehicle plate number keyboard for React (not a really keyboard, just a modal)

React 实现的车牌键盘。

## 💡 Features

- 省份 + 字母/数字 + '港澳学警领'
- 新能源车牌
- 自动判断当前位置可输入字符类型

## 🚗 Demo

[Demo](https://codesandbox.io/s/vehicle-plate-keyboard-demo-xxdlv)

![Demo](https://raw.githubusercontent.com/LiuuY/vehicle-plate-keyboard/master/demo.gif)

## 📷 Screenshots

![1](https://raw.githubusercontent.com/LiuuY/vehicle-plate-keyboard/master/screenshots/keyboard1.png)

![2](https://raw.githubusercontent.com/LiuuY/vehicle-plate-keyboard/master/screenshots/keyboard2.png)

![3](https://raw.githubusercontent.com/LiuuY/vehicle-plate-keyboard/master/screenshots/keyboard3.png)

## 📦 Installation

```Javascript
yarn add vehicle-plate-keyboard
```

## 🔨 Usage

```JavaScript
import LicenseKeyboard from 'vehicle-plate-keyboard';
import 'vehicle-plate-keyboard/dist/main.css';

...

<LicenseKeyboard
   visible={state.showKeyboard}
   onChange={value => setState({ value })}
   value={state.value}
   done={() => setState({ showKeyboard: false })}
/>
```

## 🗺 API

| props              | type                    | description                   |
| ------------------ | ----------------------- | ----------------------------- |
| visiable           | boolean                 | keyboard visible              |
| onChange           | (value: string) => void | trigger when user tap         |
| value              | string                  | controlled value              |
| done               | () => void              | trigger when keyborad dismiss |
| confirmButtonStyle | React.CSSProperties     | confirm button style          |
| confirmButtonText  | string                  | confirm button text           |
| cellTextStyle      | React.CSSProperties     | keycell style                 |
| safeArea           | boolean                 | show safearea                 |

## 🚧 Development

vehicle-plate-keyboard use [Storybook](https://storybook.js.org/) for developing in isolation.

```javascript
yarn storybook
```

open browser, http://localhost:6006/, 😆

![1](https://raw.githubusercontent.com/LiuuY/vehicle-plate-keyboard/master/screenshots/storybook.png)

## 📝 License

MIT License
