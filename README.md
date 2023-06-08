## 📗工具简介
apate是一款能够简洁、快速地对文件进行格式伪装的工具，可以在某些情况下绕过限制，如**某些大厂文件分享平台**的分享限制。  
支持**超大文件**，无需等待漫长读写，可以瞬间完成伪装或还原。  
开源项目主页：[Github: rippod/apate](https://github.com/rippod/apate)  
## 📥下载方法
1.安装运行环境：根据自己的操作系统，选择安装[.NET桌面运行时6.0（64位）](https://dotnet.microsoft.com/zh-cn/download/dotnet/thank-you/runtime-desktop-6.0.16-windows-x64-installer)或者[.NET桌面运行时6.0（32位）](https://dotnet.microsoft.com/zh-cn/download/dotnet/thank-you/runtime-desktop-6.0.16-windows-x86-installer)  
2.下载apate：[下载最新版v1.4.1](https://github.com/rippod/apate/releases/download/apate.v1.4.1/apate.v1.4.1.zip)  
## 📖使用说明
### 1. 一键伪装  
  使用预置面具文件，对真身文件进行伪装。伪装后，真身文件看起来与面具文件一样。适用大部分应用场景。  
### 2. 面具伪装  
  使用自定义面具文件，对真身文件进行伪装。伪装后，真身文件看起来与面具文件一样。适用范围取决于面具文件的选择，建议在一键伪装失效时尝试使用。  
### 3. 简易伪装  
  不使用面具文件，而是使用指定格式的二进制特征文件头，对真身文件进行伪装。伪装后，真身文件对于操作系统来说已经是指定格式，只是无法被双击执行或播放。对于EXE的简易伪装，建议真身文件不超过2G。其他格式的简易伪装适配场景较少，不建议使用。  

## ❗注意事项  
1. 使用前请务必做好数据备份。  
2. 本软件不得用于商业用途，仅做学习交流。  
3. 本软件不得用于非法用途，用户使用本软件导致的任何后果均由用户本人承担，软件作者不承担任何责任。  

## 🙋F&Q  
### 1. copy /b a.xxx +b.xxx 原理是这个吗？  
  技术上完全不同，但有类似之处。比起你说的方法有如下优点：  
  (1)针对超大文件，可以做到瞬间伪装/还原完毕，无需任何等待。  
  (2)针对文件的还原做了优化，无需知道文件的伪装面具即可一键还原。  
  (3)针对真身文件的原始文件头，做了加密处理，不易被检测出原始格式。  
### 2. 一键伪装和简易伪装有什么区别？  
  一键伪装：使用预置面具文件，对真身文件进行伪装。伪装后，真身文件看起来与面具文件一样。适用大部分应用场景。  
  简易伪装：不使用面具文件，而是使用指定格式的二进制特征文件头，对真身文件进行伪装。伪装后，真身文件对于操作系统来说已经是指定格式，只是无法被双击执行或播放。对于EXE的简易伪装，建议真身文件不超过2G。其他格式的简易伪装适配场景较少，不建议使用。  
### 3. 一键伪装只支持单一的mp4格式,建议增加多选  
  这个工具我个人使用时主要是为了解决某些大厂文件分享平台的格式限制，而这个平台对mp4格式最为宽容，所以为了方便起见我设计了这个一键伪装功能，暂不考虑增加其他选项。如果需要使用其他格式，可以使用面具伪装功能，自定义面具文件。  
