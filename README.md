# TXT to EPUB - 在线电子书转换器

纯前端 TXT 转 EPUB 工具，所有处理在浏览器本地完成，文件不会上传到任何服务器。

演示地址：https://txt2epub.937788.xyz/

## 功能

- 拖拽或点击上传 `.txt` 文件
- 支持 UTF-8、GBK、Big5、GB18030、Shift_JIS 等 10 种编码，乱码时可手动切换
- 智能识别中英文章节标题（第X章、Chapter X、楔子、序章等）
- 章节卡片展示，支持拖拽排序、合并、删除、内容编辑
- 自定义书名、作者，上传封面图片（JPG/PNG）
- 一键导出标准 EPUB 3.0 文件，兼容 Kindle、掌阅、iBooks 等主流阅读器

## 技术栈

- 纯 HTML/CSS/JavaScript，无框架依赖
- JSZip 浏览器端生成 EPUB
- TextDecoder API 处理多编码
- Canvas API 缩放封面图片

## 使用说明

1. 上传 TXT 文件，系统自动识别章节
2. 如出现乱码，切换编码格式后重新解析
3. 校对章节：拖拽排序、合并、删除、编辑内容
4. 填写书名和作者，可选上传封面
5. 点击「导出 EPUB」下载文件

## 本地运行

直接使用任意 HTTP 服务器托管即可：

```bash
python3 -m http.server 8000
```

然后访问 `http://localhost:8000`。

## 截图

![截图](截图.png)