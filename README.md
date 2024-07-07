# clf_insualance
https://www.kaggle.com/competitions/playground-series-s4e7/discussion?sort=votes

[エクセル](https://onedrive.live.com/personal/e1cd03577e8d2f8b/_layouts/15/doc2.aspx?resid=896e960f-1ea8-4b57-a743-436ddb76d5ac&cid=e1cd03577e8d2f8b&action=editnew&wdNewAndOpenCt=1719838725386&ct=1719838725996&wdOrigin=OFFICECOM-WEB.START.NEW&wdPreviousSessionSrc=HarmonyWeb&wdPreviousSession=c3b0e148-240e-4f08-8cf2-b83195904091)

# カラム

| 変数名                 | 定義                                                                                             |目的変数との相関|
|----------------------|--------------------------------------------------------------------------------------------------|-----------------|
| `id`                 | 顧客のユニークID                                                                                  |-|
| `Gender`             | 顧客の性別                                                                                         |男性の方が若干高い(女性:0.10 vs 男性0.14)|
| `Age`                | 顧客の年齢                                                                                         |30~50台は高め|
| `Driving_License`    | 0 : 顧客は運転免許を持っていない, 1 : 顧客は既に運転免許を持っている                                    |持っている方が高い(持っていない. 0.06 vs 持っている 0.12)|
| `Region_Code`        | 顧客の地域のユニークコード                                                                          |高い地域と低い地域あり(要原因追及)|
| `Previously_Insured` | 1 : 顧客は既に自動車保険に加入している, 0 : 顧客は自動車保険に加入していない                           |加入していたらほとんどなし、(0:0.22, 1: 0.00)|
| `Vehicle_Age`        | 車両の年齢                                                                                         |一年目の車:0.05, 1~2年目の車:0.18, 2年以上: 0.30 |
| `Vehicle_Damage`     | 1 : 顧客は過去に車両を損傷したことがある, 0 : 顧客は過去に車両を損傷したことがない                       |過去にありだったら: 0.25,なかったら0.00|
| `Annual_Premium`     | 顧客が年間で支払うべき保険料                                                                       |増加するにつれて、高くなる傾向あり|
| `Policy_Sales_Channel` | 顧客へのアプローチチャネルの匿名化コード（例：さまざまな代理店、メール、電話、対面など）               |経路によって複数種類あり|
| `Vintage`            | 顧客が会社に関連付けられている日数                                                                  |多少の変更あり|
| `Response`           | 1 : 顧客は興味がある, 0 : 顧客は興味がない                                                           |--|


#仮説  
・`Driving_License`=0は、比較的高齢者or 若者か
・ `Region_Code`；若者が多い地域かどうかカラム
・`Policy_Sales_Channel`ごとに刺さりやすい顧客層がありそう
・

