## 說明

這是我用Python的plotly套件做的一個互動式地圖，主要依據政府開放資料提供的[鄉鎮市區界線地圖資料](https://data.gov.tw/dataset/7441)和[社會經濟資料服務平台-108年內政大數據資料應用組競賽用資料集_村里](https://segis.moi.gov.tw/STAT/Web/Platform/QueryInterface/STAT_QueryTopProduct.aspx)，來繪製一個2019年台灣的生育率地圖。

若要觀看互動式地圖可直接下載專案內的main.html檔案。

![](https://github.com/SuYenTing/taiwan_CBR_map/blob/main/demo.gif)

## 安裝套件清單

```
pip install wheel
pip install pipwin
pipwin install numpy
pipwin install pandas
pipwin install shapely
pipwin install gdal
pipwin install fiona
pipwin install pyproj
pipwin install six
pipwin install rtree
pipwin install geopandas
pipwin install plotly
```

## 資料來源說明

若要執行程式碼，需要下載兩份資料：

1. 政府開放資料網站-[鄉鎮市區界線地圖資料](https://data.gov.tw/dataset/7441)

下載完後，需要壓縮檔內的3個檔案：

* TOWN_MOI_1091016.dbf
* TOWN_MOI_1091016.shp
* TOWN_MOI_1091016.shx

2. [社會經濟資料服務平台-108年內政大數據資料應用組競賽用資料集_村里](https://segis.moi.gov.tw/STAT/Web/Platform/QueryInterface/STAT_QueryTopProduct.aspx)，下載「行政區」頁面108年度資料

下載完後，需要壓縮檔內的1個檔案：

* 108年內政大數據資料應用組競賽用資料集_村里.csv
