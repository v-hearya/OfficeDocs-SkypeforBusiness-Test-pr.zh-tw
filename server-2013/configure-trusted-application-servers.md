﻿---
title: 設定信任的應用程式伺服器
TOCTitle: 設定信任的應用程式伺服器
ms:assetid: 20c3815f-3048-4940-8c0f-cdfcd0801d5d
ms:mtpsurl: https://technet.microsoft.com/zh-tw/library/JJ204735(v=OCS.15)
ms:contentKeyID: 49290311
ms.date: 08/10/2015
mtps_version: v=OCS.15
ms.translationtype: HT
---

# 設定信任的應用程式伺服器

 

_**上次修改主題的時間：** 2014-11-05_

在混合環境中，若您要新建立信任的應用程式伺服器，您就必須將下一個躍點集區設為 Lync Server 2013 集區。雖然，混合環境的下拉式清單中會顯示舊版 Lync Server 2010 集區和 Lync Server 2013 集區，但不支援選取舊版集區。

**建立信任的應用程式伺服器時，選取 Lync Server 2013 為下一個躍點**

1.  開啟 \[拓撲產生器\]。

2.  在左側窗格中，用滑鼠右鍵按一下 **\[信任的應用程式伺服器\]** ，然後按一下 **\[新增信任的應用程式集區\]** 。

3.  輸入信任之應用程式集區的 \[集區 FQDN\] ，然後選擇是否為單一伺服器或多部伺服器。

4.  按 **\[下一步\]** 。

5.  在 **\[選取下一個躍點\]** 頁面上，從清單中選取 Lync Server 2013 前端集區。

6.  按一下 \[完成\] 。

7.  選取最上方的 \[Lync Server\] 節點，然後從 \[動作\] 功能表中選取 \[發行\] 。
    
    驗證是否已成功地建立 \[信任的應用程式集區\] ，並關聯到正確的前端集區。

