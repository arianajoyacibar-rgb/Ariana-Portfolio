# TindaTrack

A lightweight point-of-sale and inventory app for a sari-sari store. Ring up sales, track stock, get low-stock alerts, and see what to reorder.

## Features
- **Sell**: tap an item or scan a barcode (a USB scanner types the code and presses Enter), see the total, enter cash and get the change
- **Stock**: editable stock and reorder levels, low-stock alerts, add or remove items
- **Reorder forecast**: average units sold per day over the last 7 days, days of stock left, and a suggested order quantity (a week of sales plus the reorder level, minus current stock)
- **Sales report**: today's sales and profit, a 14-day chart and best sellers
- Everything saves in the browser (`localStorage`)

## Run
Open `index.html`. The store, prices and sales history are fictional demo data generated on first load; press **Reset demo data** to regenerate them.

## Thesis angles
- Measure time per transaction and stock-count errors against a paper notebook
- Compare forecasting methods (moving average, exponential smoothing) on real sales
- Add e-wallet payment and a camera barcode scanner
