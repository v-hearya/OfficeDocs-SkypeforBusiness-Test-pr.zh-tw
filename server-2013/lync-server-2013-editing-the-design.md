﻿---
title: Lync Server 2013：編輯設計
TOCTitle: 編輯設計
ms:assetid: 08f639ba-0e5f-4ae7-9191-c3d96c25b169
ms:mtpsurl: https://technet.microsoft.com/zh-tw/library/Gg558608(v=OCS.15)
ms:contentKeyID: 52056048
ms.date: 08/10/2015
mtps_version: v=OCS.15
ms.translationtype: HT
---

# 在 Lync Server 2013 中編輯設計

 

_**上次修改主題的時間：** 2013-02-21_

在完成初始訪談問題之後，即可編輯網站的完整網域名稱 (FQDN) 與 IP 位址。若要執行此作業，請在「全域拓撲」 頁面上連按兩下要編輯的網站。

規劃工具會顯示所選網站的站台拓撲。在網站頁面的底部有四個索引標籤：

![規劃工具的站台拓撲](images/Gg558608.e6189c20-360a-42bd-ba90-11bdb5b7551b(OCS.15).jpg "規劃工具的站台拓撲")

  - 站台拓撲 – 目前顯示頁面具有如同建議的可見拓撲概觀。

  - Edge 網路圖 –「Edge 網路圖」頁面是設計人員在 規劃工具 中執行大部分工作的地方。圖中顯示建議之 Lync Server 2013 拓撲的網路組態，其中包含伺服器、集區及負載平衡器 (硬體和網域名稱系統 (DNS) 兩者) 的可編輯 IP 位址和 FQDN 項目 。

  - Edge Admin 報表 – \[Edge Admin 報表\] 總共包含四份報表：
    
    ![Edge 管理員報告頁面](images/Gg558608.0019cc5e-af39-4cb9-82ce-58f6388242ff(OCS.15).jpg "Edge 管理員報告頁面")  
    
      - 摘要報表 – 網路組態設定的一般報表。如果您編輯「Edge 網路圖」頁面上將用於實際部署的拓撲 TCP/IP 和 FQDN 值，則這些位址和名稱會在此顯現，否則會顯示預設文字。
    
      - 憑證報表 – 憑證報表會列出拓撲所需憑證的主體名稱和主體替代名稱。
    
      - 防火牆報表 – 防火牆報表會列出在基礎結構中設定周邊防火牆所需的資訊。其中包含 IP 位址 (預設值或編輯過的值)、伺服器角色、來源 IP 和連接埠、目的地 IP 和連接埠、傳輸通訊協定、應用程式通訊協定以及相關附註。
    
      - DNS 報表 – DNS 報表會列出所應建立之 DNS 項目的相關資訊。其中包含正常運作所需的記錄類型、FQDN、IP 位址及註解。

  - 網站摘要 – 網站摘要會概要呈現您在回答初始訪談問題或填入 \[設計網站\] 中的值時所做之選擇。也會呈現容量資訊。
    
    <table>
    <thead>
    <tr class="header">
    <th><img src="images/Gg398811.note(OCS.15).gif" title="note" alt="note" />附註：</th>
    </tr>
    </thead>
    <tbody>
    <tr class="odd">
    <td>[網站摘要] 頁面上的資訊是針對各項設計所自訂的，無法包含此處詳述的所有區段或資訊。</td>
    </tr>
    </tbody>
    </table>


## 請參閱

#### 概念

[編輯網路組態圖](lync-server-2013-editing-the-network-configuration-diagram.md)
