# Döviz, Borsa ve Kripto Paralar API Servisleri
Bulunan Tüm Döviz Kurları, Borsa ve Kripto Fiyatları Toplu API Servisleri
```
sizin bulduklarınız da varsa eğer Discussions kısmından iletebilirsiniz.
```

## midas döviz api - tarih: 2025.10.10
- URL: https://www.getmidas.com/wp-json/midas-api/v1/midas_table_data?sortId=&return=doviz
- Örnek Döviz JSON
```json
[
  {
    "_id": "o10",
    "Code": "USDTRY",
    "Open": 41.7562,
    "High": 41.8222,
    "Low": 41.7234,
    "Last": 41.8122,
    "Close": 41.8122,
    "PreviousClose": 41.7439,
    "DateTime": 1760044474041,
    "DailyChange": 0.0683,
    "DailyChangePercent": 0.16,
    "Ask": 41.8216,
    "Bid": 41.8029,
    "YearlyChange": 6.4411
  },
  {
    "_id": "o11",
    "Code": "EURTRY",
    "Open": 48.4224,
    "High": 48.4224,
    "Low": 48.2867,
    "Last": 48.3363,
    "Close": 48.3363,
    "PreviousClose": 48.429,
    "DateTime": 1760044470042,
    "DailyChange": -0.0927,
    "DailyChangePercent": -0.19,
    "Ask": 48.4485,
    "Bid": 48.2241,
    "YearlyChange": 11.6776
  },
  {
    "_id": "o865",
    "Code": "GBPTRY",
    "Open": 55.6712,
    "High": 55.6712,
    "Low": 55.5774,
    "Last": 55.6072,
    "Close": 55.6072,
    "PreviousClose": 55.6712,
    "DateTime": 1760044469961,
    "DailyChange": -0.064,
    "DailyChangePercent": -0.11,
    "Ask": 55.6955,
    "Bid": 55.519,
    "YearlyChange": 11.3063
  }
]
```

## midas borsa (bist) api - tarih: 2025.10.10
- URL: https://www.getmidas.com/wp-json/midas-api/v1/midas_table_data?sortId=&return=table
- Örnek Borsa BIST JSON
```json
[
    {
        "_id": "c138",
        "Code": "XU100",
        "Name": "BIST 100",
        "Last": 10726.98,
        "DailyChange": -29.29,
        "DailyChangePercent": -0.27,
        "DateTime": 1760020200000,
        "Ask": 0,
        "Bid": 0,
        "High": 10785.45,
        "Low": 10714.4,
        "PreviousClose": 10756.27,
        "YearlyChange": 2697.83,
        "WeeklyChange": -73.69,
        "MonthlyChange": 462.62,
        "YearlyChangePercent": 33.59,
        "WeeklyChangePercent": -0.68,
        "MonthlyChangePercent": 4.51
    },
    {
        "_id": "h115",
        "Code": "EREGL",
        "Name": "EREGLI DEMIR CELIK",
        "Last": 43.1,
        "DailyChange": -0.32,
        "DailyChangePercent": -0.74,
        "DateTime": 1760020200000,
        "Ask": 43.1,
        "Bid": 43.08,
        "High": 43.56,
        "Low": 43.04,
        "PreviousClose": 43.42,
        "YearlyChange": 0,
        "WeeklyChange": -0.16,
        "MonthlyChange": -3.52,
        "YearlyChangePercent": 0,
        "WeeklyChangePercent": -0.37,
        "MonthlyChangePercent": -7.56
    }
]
```

## Paragaranti Foreks API
- BIST Endeks Listesi: https://web-paragaranti-pubsub.foreks.com/web-services/securities/exchanges/BIST/groups/E
- BIST Endes Alfabetik Detaylı Liste: https://web-paragaranti-pubsub.foreks.com/web-services/securities?key=A&index=&exchangeGroupFilter=BIST.E&extendedResult=true ( * key=**HARF** )
- BIST Endeks Detayı: https://web-paragaranti-pubsub.foreks.com/web-services/securities/definition?name=ENDEKS_ISMI&group=E&exchange=BIST (**ENDEKS_ISMI** yazan bölüme bir üst satırlardaki Endeks isimleri gelecektir.)
- BIST Yatırım Kuruluşları Listesi: https://web-paragaranti-pubsub.foreks.com/web-services/securities/exchanges/BIST/groups/I

- Serbest Piyasa Dolar Tarihsel Verileri: https://web-paragaranti-pubsub.foreks.com/web-services/historical-data?userName=undefined&name=SUSD&exchange=FREE&market=N&group=F&last=300&period=1440&intraPeriod=null&isLast=false&from=20180508000000&to=20181108235900 (**Tarih aralığını belirtmeyi unutmayınız.**)
- Serbest Piyasa Euro Tarihsel Verileri: https://web-paragaranti-pubsub.foreks.com/web-services/historical-data?userName=undefined&name=SEUR&exchange=FREE&market=N&group=F&last=300&period=1440&intraPeriod=null&isLast=false&from=20180508000000&to=20181108235900 (**Tarih aralığını belirtmeyi unutmayınız.**)
- Serbest Piyasa Sterlin Tarihsel Verileri: https://web-paragaranti-pubsub.foreks.com/web-services/historical-data?userName=undefined&name=SGBP&exchange=FREE&market=N&group=F&last=300&period=1440&intraPeriod=null&isLast=false&from=20180508000000&to=20181108235900 (**Tarih aralığını belirtmeyi unutmayınız.**)

* Tarihsel verilere **name** değişkenine diğer kur isimlerini ekleyerek kontrol edebilirsiniz.


## Hürriyet Bigpara Api
- Hisse Listesi: http://bigpara.hurriyet.com.tr/api/v1/hisse/list
- Hisse Detay: http://bigpara.hurriyet.com.tr/api/v1/borsa/hisseyuzeysel/AEFES (*AEFES temsili değerdir, bir üst satırdaki **kod** verisi kullanılacaktır.)


---
## canlidoviz.com Api (iptal, çalışmıyor) - Güncelleme: 2025 
- Döviz: https://canlidoviz.com/doviz-kurlari.jsonld
- Altın: https://canlidoviz.com/altin-fiyatlari.jsonld
- Kripto: https://canlidoviz.com/kripto-paralar.jsonld
- Borsa: https://canlidoviz.com/borsa.jsonld
- Pariteler: https://canlidoviz.com/pariteler.jsonld
- Emtia: https://canlidoviz.com/emtia-fiyatlari.jsonld
- Endeks: https://canlidoviz.com/endeks.jsonld
