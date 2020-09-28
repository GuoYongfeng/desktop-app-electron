# 远程会议系统桌面端

## 安装

安装下载 `electron` 比较耗时，大概得 5 分钟左右。

```bash
yarn install
```

## 开发



```bash
yarn dev
```

## 生产环境打包


```bash
yarn package
```

## 涉及主要技术点

- main process & renderer process
- electron
	- remote、ipc
	- BowserWindow
	- dialog 对话框
	- desktopCapturer捕获音频和视频流 https://www.electronjs.org/docs/api/desktop-capturer、https://blog.csdn.net/dqm159159/article/details/107077224/
	- electron-store 数据持久化，缓存、状态、用户信息。存在在json file，app.getPath
	- electron-builder 打包和安装盘
	- electron-screen-recorder 录屏，https://www.cnblogs.com/olivers/p/12609427.html
	- WebRTC navigator.getUserMedia() 打开电脑摄像头及麦克风

- react-dom
- react
- create-react-app BROWSER=none
- tools
	- npx
	- electron-is-dev
	- nodemon node文件watch
	- Devtron 开发调试工具
	- concurrently
	- wait-on
	- cross-env
- require -》window.require
- promise
- nodejs
	- fs 
	- promises
	- path
