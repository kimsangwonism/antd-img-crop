# antd-img-crop

图片裁切工具，用于 Ant Design [Upload](https://ant.design/components/upload-cn/) 组件。

[![npm](https://img.shields.io/npm/v/antd-img-crop.svg?style=flat-square)](https://www.npmjs.com/package/antd-img-crop)
[![npm](https://img.shields.io/npm/dt/antd-img-crop?style=flat-square)](https://www.npmtrends.com/antd-img-crop)
[![npm bundle size](https://img.shields.io/bundlephobia/minzip/antd-img-crop?style=flat-square)](https://bundlephobia.com/result?p=antd-img-crop)
[![GitHub](https://img.shields.io/github/license/nanxiaobei/antd-img-crop?style=flat-square)](https://github.com/nanxiaobei/antd-img-crop/blob/master/LICENSE)

[English](./README.md) | 简体中文

## 示例

[![Edit antd-img-crop](https://codesandbox.io/static/img/play-codesandbox.svg)](https://codesandbox.io/s/antd-img-crop-4qoom5p9x4?fontsize=14)

## 安装

```sh
yarn add antd-img-crop
```

## 使用

```jsx harmony
import ImgCrop from 'antd-img-crop';
import { Upload } from 'antd';

const Demo = () => (
  <ImgCrop>
    <Upload>+ Add image</Upload>
  </ImgCrop>
);
```

## Props

| 属性        | 类型                 | 默认         | 说明                                           |
| ----------- | -------------------- | ------------ | ---------------------------------------------- |
| aspect      | `number`             | `1 / 1`      | 裁切区域宽高比，`width / height`               |
| shape       | `string`             | `'rect'`     | 裁切区域形状，`'rect'` 或 `'round'`            |
| grid        | `boolean`            | `false`      | 显示裁切区域网格（九宫格）                     |
| zoom        | `boolean`            | `true`       | 启用图片缩放                                   |
| rotate      | `boolean`            | `false`      | 启用图片旋转                                   |
| beforeCrop  | `function`           | -            | 弹窗打开前调用，若返回 `false`，弹框将不会打开 |
| modalTitle  | `string`             | `'编辑图片'` | 弹窗标题                                       |
| modalWidth  | `number` \| `string` | `520`        | 弹窗宽度，像素值或百分比                       |
| modalOk     | `string`             | `'确定'`     | 弹窗确定按钮文字                               |
| modalCancel | `string`             | `'取消'`     | 弹窗取消按钮文字                               |

## 样式

为防止覆盖自定义 `antd` 样式，`antd-img-crop` 中没有引入组件样式文件。

因此如果你的项目配置了 `babel-plugin-import`，且未使用 `Modal` 或 `Slider`，则需自行引入样式：

```js
import 'antd/es/modal/style';
import 'antd/es/slider/style';
```

## 协议

[MIT License](https://github.com/nanxiaobei/antd-img-crop/blob/master/LICENSE) (c) [nanxiaobei](https://mrlee.me/)
