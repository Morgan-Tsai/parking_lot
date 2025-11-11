# 練習專案七:小小停車場

## 簡介

這個專案「小小停車場」透過 `gradio` 與 `easyocr` 模組製作出一個以秒計費的停車場網頁應用程式。我們使用了 `easyocr` 進行車牌辨識，透過 Python 函數與標準模組進行概念驗證，並以 `gradio` 的介面做出成品。

## 專案亮點

- 使用 `datetime` 操作日期時間與格式調整。
- 以 `easyocr` 做光學字元辨識。
- 以 `gradio` 做出成品。
- 成品能夠以 Hugging Face Spaces 網址直接訪問,可以透過 Hugging Face Spaces 的連結:  參考成品。
- 可以重現（Reproducible）。

## 如何重現

- 安裝 [Miniconda](https://docs.anaconda.com/miniconda)
- 依據 `environment.ym`l 建立環境：

```bash
conda env create -f environment.yml
```

- 將 `data/` 資料夾中的 `car_plate_1.jpg`、`car_plate_2.jpg` 與 `car_plate_3.jpg` 放置於專案資料夾的 `data/` 資料夾中。
- 啟動環境並執行 `python app.py` 並前往 `http://127.0.0.1:7860` 瀏覽成品。