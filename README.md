# 图片裁切压缩工具

一个运行在浏览器里的图片裁切与压缩工具。支持批量上传图片、自由裁切、固定比例裁切、常用证件照尺寸、图片基础调整，并可以按原图百分比或指定文件大小导出结果。

项目是纯前端静态页面，不需要后端服务，适合直接部署到 GitHub Pages。

## 在线访问

GitHub Pages 地址：

https://kenguinping.github.io/image-crop-by-KP/

项目仓库：

https://github.com/KenguinPing/image-crop-by-KP

## 功能特点

- 支持上传单张或多张图片，也可以多次添加图片到队列
- 支持点击或拖拽上传图片
- 支持在图片队列中切换当前裁切图片
- 支持从队列中移除不需要的图片
- 支持自由裁切和常用固定比例裁切
- 支持 `1:1`、`4:3`、`3:2`、`2:3`、`16:9`、`9:16`
- 支持常用证件照预设，包括身份证、护照和常见签证尺寸
- 支持手动输入裁切比例或目标分辨率
- 支持按原图百分比压缩输出
- 支持按绝对文件大小压缩输出
- 支持导出 `JPEG`、`PNG`、`WebP`
- 支持黑白、反色、曝光、对比度、色温、饱和度调整
- 支持浅色、深色、猛男mode 三种主题
- 支持等待下载区，多张结果可勾选后批量下载

## 使用方法

1. 打开网页。
2. 点击上传区域，或把图片拖到页面中。
3. 如果上传了多张图片，在左侧图片队列里选择要处理的图片。
4. 选择裁切比例，或使用自由裁切。
5. 拖动裁切框调整裁切区域。
6. 根据需要调整图片效果。
7. 设置输出文件大小和输出格式。
8. 点击“生成图片”。
9. 在等待下载区选择需要下载的结果。
10. 点击“下载结果”保存图片。

## 本地运行

这个项目是静态网页，直接打开 `index.html` 就可以使用。

也可以用本地服务器运行：

```bash
python -m http.server 8080
```

然后在浏览器打开：

```text
http://127.0.0.1:8080/
```

## 部署到 GitHub Pages

1. 把 `index.html`、`README.md` 和 `assets/` 文件夹上传到 GitHub 仓库。
2. 进入仓库的 `Settings`。
3. 找到 `Pages`。
4. 在 `Build and deployment` 里选择：
   - Source: `Deploy from a branch`
   - Branch: `main`
   - Folder: `/ (root)`
5. 点击 `Save`。
6. 等待 GitHub Pages 构建完成。

部署完成后，网站一般会显示在：

```text
https://你的用户名.github.io/仓库名/
```

## 项目结构

```text
.
├── index.html
├── README.md
└── assets/
    ├── dark-bg.jpg
    ├── eva-bg.jpg
    ├── kenguinping-avatar.jpg
    ├── light-bg.jpg
    └── mengnan-bg.jpg
```

## 技术说明

- 使用 HTML、CSS 和 JavaScript 编写
- 使用 Canvas 完成图片预览、裁切和导出
- 所有图片处理都在浏览器本地完成
- 不会把上传的图片发送到服务器

## 作者

created by KenguinPing

