# 温馨提示卡片应用 - 公网部署版本

这是一个带有自定义背景图片的温馨提示卡片生成器，可以部署到任何静态网站托管服务。

## 文件结构
```
public/
├── index.html (主应用文件)
├── images/
│   ├── background.png (页面背景图片)
│   ├── card1.png (卡片背景图片)
│   └── README.md (图片使用说明)
└── README.md (本文件)
```

## 部署到GitHub Pages

1. 在GitHub上创建一个新的仓库
2. 将public文件夹中的所有文件上传到仓库
3. 在仓库设置中启用GitHub Pages功能
4. 选择根目录作为GitHub Pages源
5. 保存设置，您的应用将在几分钟内上线

## 部署到Vercel

1. 访问 [vercel.com](https://vercel.com/)
2. 注册或登录您的账户
3. 点击"New Project"
4. 导入您的项目或直接上传public文件夹
5. Vercel会自动检测这是一个静态网站并进行部署
6. 部署完成后，您将获得一个公开访问的URL

## 部署到Netlify

1. 访问 [netlify.com](https://netlify.com/)
2. 注册或登录您的账户
3. 点击"New site from Git"或"Drag and drop your site folder here"
4. 选择您的Git仓库或直接拖拽public文件夹
5. Netlify会自动进行部署
6. 部署完成后，您将获得一个公开访问的URL

## 自定义图片

### 页面背景图片
- 替换 `images/background.png` 文件来自定义页面背景
- 推荐尺寸: 1920x1080 像素或更大
- 格式: PNG, JPG, WebP

### 卡片背景图片
- 替换 `images/card1.png` 文件来自定义卡片背景
- 推荐尺寸: 300x200 像素左右
- 格式: PNG, JPG, WebP

### 添加更多卡片背景图片
1. 在 `images` 文件夹中添加更多图片文件 (如 `card2.png`, `card3.png` 等)
2. 修改 `index.html` 文件中的JavaScript部分:
   ```javascript
   // 定义自定义图片数组
   const customImages = [
       './images/card1.png',
       './images/card2.png',  // 添加新图片
       './images/card3.png',  // 添加新图片
       // ...
   ];
   ```

## 技术说明

- 纯前端实现，无后端依赖
- 使用HTML5, CSS3和原生JavaScript
- 响应式设计，适配移动设备
- 支持触摸操作