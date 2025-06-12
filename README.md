<div align="center">
  <img src="resource/logo_big.png" width="300" style="margin-right: 3000px;"/> 
</div>

<h1 align="center">
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;EPUB下載器
</h1>

[文庫吧/輕小說文庫](www.wenku8.net)(wenku8)網站小說下載，EPUB打包。

特性：

* Fluent Design風格介面，下載進度與書籍封面顯示，主題切換，下載目錄自定義。
* 前後端分離，同時支援命令列版本。
* EPUB格式打包，支援多種閱讀器。
* 插圖排版。
* 書籍批次下載。
* 圖片多執行緒下載。
* 缺失連結自動修復。
* 自定義彩頁。
* ...................

有建議或bug可以提issue，由於軟體更新頻繁，可以加QQ群獲得更多資訊：563072544

圖形介面使用 [PyQt-Fluent-Widgets](https://pyqt-fluent-widgets.readthedocs.io/en/latest/index.html) 介面編寫。

[release](https://github.com/ShqWW/lightnovel-download/releases/tag/downloader) 頁面發布了已經打包好的exe可執行程式，包括圖形化版本和命令列版本（系統最低要求Windows 10）。

介面樣例：
<div align="center">
  <img src="resource/example1.png" width="400"/>
  <img src="resource/example2.png" width="400"/>
</div>

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
```
pyinstaller -F -w -i .\resource\logo.png --paths=C:\Users\haoru\bilinovel-download .\lightnovel_gui.py --clean
```
```
pyinstaller -F -i .\resource\logo.png --paths=C:\Users\haoru\bilinovel-download .\lightnovel.py --clean
```

## FAQ
若遇上`输入卷号超过实际卷数！`的錯誤，請連上香港的VPN再下載

## 相關專案：

* [輕小說文庫EPUB下載器](https://github.com/ShqWW/lightnovel-download)
* [哔哩輕小說EPUB下載器](https://github.com/ShqWW/bilinovel-download)
* [拷貝漫畫EPUB下載器](https://github.com/ShqWW/copymanga-download)

## EPUB書籍編輯和管理工具推薦：
1. [Sigil](https://sigil-ebook.com/) 
2. [Calibre](https://www.calibre-ebook.com/)