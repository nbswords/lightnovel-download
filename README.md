<div align="center">
  <img src="resource/logo_big.png" width="300" style="margin-right: 3000px;"/> 
</div>

<h1 align="center">
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;EPUB下載器
</h1>

[文庫吧/輕小說文庫](www.wenku8.net)(wenku8)網站小說下載，EPUB打包。

介面樣例：
<div align="center">
  <img src="resource/example1.png" width="400"/>
  <img src="resource/example2.png" width="400"/>
</div>

## 介紹

鑒於原版repo已無法正常抓取，本repo使用selenium改寫了原版的抓取功能來繞過Cloudflare，功能基本相同
- [release](https://github.com/nbswords/lightnovel-download/releases)有打包好的exe可執行程式（系統最低要求Windows 10）
- 若遇上`输入卷号超过实际卷数！`的錯誤，請連上香港VPN後再重新執行
- 由於`cloudscraper`也無法繞過輕小說文庫的Cloudflare，因此使用selenium，但selenium的缺點就是很慢，平均下載一本小說需要5~10分鐘左右，若覺得還有改進的空間歡迎提PR

## 使用前安裝需要的套件
```
pip install -r requirements.txt -i https://pypi.org/simple/
```
## 使用終端機模式執行：
```
python bilinovel.py
```

## 使用圖形介面執行:
```
python bilinovel_gui.py
```

## 使用pyinstaller打包:
```
pip install pyinstaller
```
### 圖形介面
```
pyinstaller -F -w -i resource/logo.png --paths=./lightnovel-download lightnovel_gui.py --clean
```
### 終端機
```
pyinstaller -F -i resource/logo.png --paths=./lightnovel-download lightnovel.py --clean
```
