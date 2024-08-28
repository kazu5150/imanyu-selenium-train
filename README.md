# Selenium Webスクレイピングプロジェクト

このプロジェクトは、Jupyter Lab環境でPythonを使用してSelenium WebDriverによるWebスクレイピングを行うものです。

⭐️⭐️ChromeDriverManager を使って、いつも最新のchromeDriverをインストールする仕組みを使っています。



## 環境設定

このプロジェクトは、環境管理にAnacondaを使用しています。環境をセットアップするには：

1. 新しいConda環境を作成します：
   ```
   conda create --name selenium_env python=3.8
   ```

2. 環境をアクティベートします：
   ```
   conda activate selenium_env
   ```

3. 必要なパッケージをインストールします：
   ```
   conda install selenium jupyter
   pip install webdriver-manager
   ```

## プロジェクト構成

- `web_scraping.ipynb`: スクレイピングコードを含むメインのJupyterノートブック
- `README.md`: このファイル。プロジェクト情報とセットアップ手順を含みます

## 使用方法

1. Conda環境がアクティベートされていることを確認します：
   ```
   conda activate selenium_env
   ```

2. Jupyter Labを起動します：
   ```
   jupyter lab
   ```

3. `web_scraping.ipynb`ノートブックを開き、セルを実行してWebスクレイピングタスクを実行します。


## コード例
from selenium import webdriver
from selenium.webdriver.chrome.service import Service
from webdriver_manager.chrome import ChromeDriverManager
from selenium.webdriver.common.by import By
import time

print(f"Selenium version: {selenium.__version__}")
　###Selenium version: 4.31.1

 ###seleniumのバージョンはSelenium 4.0であり必要があります。  




## 注意事項

- このプロジェクトはChromeDriverを使用するため、Chromeブラウザがインストールされていることを確認してください。
- `webdriver-manager`パッケージを使用して、適切なバージョンのChromeDriverを自動的に管理しています。
- スクレイピングを行う際は、ウェブサイトの利用規約とrobots.txtファイルを尊重してください。

## 貢献

このリポジトリをフォークして、改善やバグ修正のためのプルリクエストを提出していただけると幸いです。

## ライセンス

[ここに選択したライセンスを記載してください]