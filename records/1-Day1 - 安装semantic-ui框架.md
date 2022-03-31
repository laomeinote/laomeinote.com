## 1. Day1 - 安装semantic-ui框架

准备条件：

- 安装npm
- 安装nodejs

```bash
PS D:\Project\laomeinote.com> npm -v
6.14.12
PS D:\Project\laomeinote.com> node -v
v14.16.1
```

前端模板框架还是放到static目录里去开发。

在这里安装node依赖包。

### 安装gulp

```bash
cd static

npm install -g gulp

npm install gulp --save-dev
```

### 安装semantic-ui

由于semantic-ui主线开发已经停了很久，故使用fomantic-ui。

```bash
npm install fomantic-ui --save
```

之后弹出对话框：

```bash
[22:30:41] Starting 'run setup'...
? Set-up Semantic UI (Use arrow keys)
> Automatic (Use default locations and all components)
  Express (Set components and output folder)
  Custom (Customize all src/dist values)
```

选择第一个Automatic后进入下一步，

```bash
[22:30:41] Starting 'run setup'...
? Set-up Semantic UI Automatic (Use default locations and all components)
? We detected you are using NPM Nice! Is this your project folder? D:\Project\laomeinote.com\static (Use arrow keys)
> Yes
  No, let me specify
```

选择Yes，进入下一步，

```bash
[22:30:41] Starting 'run setup'...
? Set-up Semantic UI Automatic (Use default locations and all components)
? We detected you are using NPM Nice! Is this your project folder? D:\Project\laomeinote.com\static Yes
? Where should we put Semantic UI inside your project? (semantic/)
```

选择默认目录即可，完成后在目录下会生成semantic目录与semantic.json文件，进入编译。

```bash
cd semantic

gulp build
```

编译好的semantic ui会在dist目录下，生成如下文件。

```bash
D:\Project\laomeinote.com\static\semantic\dist$ tree
.
├── components
│   ├── accordion.css
│   ├── accordion.js
│   ├── accordion.min.css
│   ├── accordion.min.js
│   ├── ad.css
│   ├── ad.min.css
│   ├── api.js
│   ├── api.min.js
│   ├── breadcrumb.css
│   ├── breadcrumb.min.css
│   ├── button.css
│   ├── button.min.css
│   ├── calendar.css
│   ├── calendar.js
│   ├── calendar.min.css
│   ├── calendar.min.js
│   ├── card.css
│   ├── card.min.css
│   ├── checkbox.css
│   ├── checkbox.js
│   ├── checkbox.min.css
│   ├── checkbox.min.js
│   ├── comment.css
│   ├── comment.min.css
│   ├── container.css
│   ├── container.min.css
│   ├── dimmer.css
│   ├── dimmer.js
│   ├── dimmer.min.css
│   ├── dimmer.min.js
│   ├── divider.css
│   ├── divider.min.css
│   ├── dropdown.css
│   ├── dropdown.js
│   ├── dropdown.min.css
│   ├── dropdown.min.js
│   ├── embed.css
│   ├── embed.js
│   ├── embed.min.css
│   ├── embed.min.js
│   ├── emoji.css
│   ├── emoji.min.css
│   ├── feed.css
│   ├── feed.min.css
│   ├── flag.css
│   ├── flag.min.css
│   ├── form.css
│   ├── form.js
│   ├── form.min.css
│   ├── form.min.js
│   ├── grid.css
│   ├── grid.min.css
│   ├── header.css
│   ├── header.min.css
│   ├── icon.css
│   ├── icon.min.css
│   ├── image.css
│   ├── image.min.css
│   ├── input.css
│   ├── input.min.css
│   ├── item.css
│   ├── item.min.css
│   ├── label.css
│   ├── label.min.css
│   ├── list.css
│   ├── list.min.css
│   ├── loader.css
│   ├── loader.min.css
│   ├── menu.css
│   ├── menu.min.css
│   ├── message.css
│   ├── message.min.css
│   ├── modal.css
│   ├── modal.js
│   ├── modal.min.css
│   ├── modal.min.js
│   ├── nag.css
│   ├── nag.js
│   ├── nag.min.css
│   ├── nag.min.js
│   ├── placeholder.css
│   ├── placeholder.min.css
│   ├── popup.css
│   ├── popup.js
│   ├── popup.min.css
│   ├── popup.min.js
│   ├── progress.css
│   ├── progress.js
│   ├── progress.min.css
│   ├── progress.min.js
│   ├── rail.css
│   ├── rail.min.css
│   ├── rating.css
│   ├── rating.js
│   ├── rating.min.css
│   ├── rating.min.js
│   ├── reset.css
│   ├── reset.min.css
│   ├── reveal.css
│   ├── reveal.min.css
│   ├── search.css
│   ├── search.js
│   ├── search.min.css
│   ├── search.min.js
│   ├── segment.css
│   ├── segment.min.css
│   ├── shape.css
│   ├── shape.js
│   ├── shape.min.css
│   ├── shape.min.js
│   ├── sidebar.css
│   ├── sidebar.js
│   ├── sidebar.min.css
│   ├── sidebar.min.js
│   ├── site.css
│   ├── site.js
│   ├── site.min.css
│   ├── site.min.js
│   ├── slider.css
│   ├── slider.js
│   ├── slider.min.css
│   ├── slider.min.js
│   ├── state.js
│   ├── state.min.js
│   ├── statistic.css
│   ├── statistic.min.css
│   ├── step.css
│   ├── step.min.css
│   ├── sticky.css
│   ├── sticky.js
│   ├── sticky.min.css
│   ├── sticky.min.js
│   ├── tab.css
│   ├── tab.js
│   ├── tab.min.css
│   ├── tab.min.js
│   ├── table.css
│   ├── table.min.css
│   ├── text.css
│   ├── text.min.css
│   ├── toast.css
│   ├── toast.js
│   ├── toast.min.css
│   ├── toast.min.js
│   ├── transition.css
│   ├── transition.js
│   ├── transition.min.css
│   ├── transition.min.js
│   ├── visibility.js
│   └── visibility.min.js
├── semantic.css
├── semantic.js
├── semantic.min.css
├── semantic.min.js
└── themes
    ├── basic
    │   └── assets
    │       └── fonts
    │           ├── icons.eot
    │           ├── icons.svg
    │           ├── icons.ttf
    │           └── icons.woff
    ├── default
    │   └── assets
    │       ├── fonts
    │       │   ├── brand-icons.eot
    │       │   ├── brand-icons.svg
    │       │   ├── brand-icons.ttf
    │       │   ├── brand-icons.woff
    │       │   ├── brand-icons.woff2
    │       │   ├── icons.eot
    │       │   ├── icons.svg
    │       │   ├── icons.ttf
    │       │   ├── icons.woff
    │       │   ├── icons.woff2
    │       │   ├── outline-icons.eot
    │       │   ├── outline-icons.svg
    │       │   ├── outline-icons.ttf
    │       │   ├── outline-icons.woff
    │       │   └── outline-icons.woff2
    │       └── images
    │           └── flags.png
    ├── github
    │   └── assets
    │       └── fonts
    │           ├── octicons-local.ttf
    │           ├── octicons.svg
    │           ├── octicons.ttf
    │           └── octicons.woff
    └── material
        └── assets
            └── fonts
                ├── icons.eot
                ├── icons.svg
                ├── icons.ttf
                ├── icons.woff
                └── icons.woff2
```

