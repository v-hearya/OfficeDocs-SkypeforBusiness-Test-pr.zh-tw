﻿---
title: Lync Server 2013：PSTN 閘道位置
TOCTitle: PSTN 閘道位置
ms:assetid: 49693a35-fad3-49ee-a71e-c7e4537b79aa
ms:mtpsurl: https://technet.microsoft.com/zh-tw/library/JJ994031(v=OCS.15)
ms:contentKeyID: 52056119
ms.date: 08/10/2015
mtps_version: v=OCS.15
ms.translationtype: HT
---

# Lync Server 2013 中 PSTN 閘道的位置

 

_**上次修改主題的時間：** 2013-03-09_

透過 PSTN 閘道和 PBX 路由傳送的通話可能需要位置基礎路由限制，視此類系統的位置而定。位置基礎路由可於資料粒度層級依個別主幹啟用。

於主幹上啟用位置基礎路由時，會引進下列的一組規則：

  - 當位置基礎路由依個別主幹啟用時，於該主幹上定義的規則將只會套用到透過該主幹路由傳送的通話。

  - 為於通話來自非 PSTN 閘道所在網站時禁止 PSTN 免話費機制，位置基礎路由引進了網站與特定主幹之間的關聯性。此規則會定義允許將通話路由傳送到特定主幹的網站。

主幹可以使用兩種方式啟用位置基礎路由：

  - 針對將通話輸出到 PSTN 的 PSTN 閘道定義主幹。由此類型主幹路由傳送的傳入通話，將只會路由傳送到與主幹位於相同網站內的端點。

  - 針對不會將通話輸出至 PSTN 及於固定位置使用舊式電話 (亦即 PBX 電話) 之服務使用者的 中繼伺服器 對等端定義主幹。對於此一特殊組態，所有由此類型主幹路由傳送的傳入通話，都將被視為來自主幹所在網站。會為來自 PBX 使用者的通話執行位置基礎路由，與位於主幹所在網站的 Lync 使用者處理方式相同。如果兩個位於不同網站的 PBX 系統透過 Lync Server 連接，則位置基礎路由會允許從特定網站上的某個 PBX 端點，路由傳送到位於其他網站的另一個 PBX 端點。此案例不會受到位置基礎路由的封鎖。除此之外，於類似情況下，當 Lync 使用者位於相同位置，連接到具有此組態之 中繼伺服器 對等端的端點，將能夠撥打電話給不論 中繼伺服器 對等端關聯的網站為何，皆不會將通話路由傳送到 PSTN (亦即連接到不同 PBX 的端點) 的其他 中繼伺服器 對等端 (也可以接聽對方來電)。所有涉及 PSTN 端點的輸入通話、輸出通話、通話轉接和來電轉接，都將受到位置基礎路由支配，僅能使用定義為此類 中繼伺服器 對等端之本機閘道之 PSTN 閘道。

## 請參閱

#### 其他資源

[Lync Server 2013 中的位置基礎路由指引](lync-server-2013-guidance-for-location-based-routing.md)

