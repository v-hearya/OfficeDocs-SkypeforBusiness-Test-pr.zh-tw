﻿---
title: 為使用者設定電話語音
TOCTitle: 為使用者設定電話語音
ms:assetid: 4546432e-c839-4517-a2c5-bc0d4d8c6a03
ms:mtpsurl: https://technet.microsoft.com/zh-tw/library/Gg520988(v=OCS.15)
ms:contentKeyID: 49290768
ms.date: 08/10/2015
mtps_version: v=OCS.15
ms.translationtype: HT
---

# 為使用者設定電話語音

 

_**上次修改主題的時間：** 2012-11-01_

電話語音設定是可在使用者的 Lync Server 控制台中設定的使用者帳戶的一些個別設定 (亦即，如果 Lync Server 2013 已啟用個別使用者，且組織支援電話語音)。

Lync Server 使用者電話語音選項包括：

  - **音訊/視訊已停用**   使用者無法撥打音訊和視訊電話。

  - **僅限電腦對電腦**   使用者只能撥打電腦對電腦音訊或視訊電話。

  - **企業語音**   使用者可以利用 Lync Server 2013 基礎結構來路由所有來電和撥出的電話。使用者也可以進行電腦對電腦呼叫。

  - **遠端呼叫控制**   使用者可以利用 Lync Server 2013 來控制桌上電話，也可以進行電腦對電腦呼叫。

如需設定組織的電話語音的詳細資訊，請參閱部署移轉文件[為使用者設定電話語音](lync-server-2013-configure-telephony-for-a-user.md)＞及＜[在 Lync Server 2013 中部署企業語音](lync-server-2013-deploying-enterprise-voice.md)＞。

## 若要設定特定使用者帳戶的電話語音

1.  使用指派給 CsUserAdministrator 角色或 CsAdministrator 角色的使用者帳戶，登入內部部署中的任何電腦。

2.  開啟瀏覽器視窗，然後輸入管理 URL 以開啟 Lync Server 控制台。如需可用於啟動 Lync Server 控制台的不同方法的詳細資料，請參閱[開啟 Lync Server 系統管理工具](lync-server-2013-open-lync-server-administrative-tools.md)。

3.  在左導覽列中，按一下 **\[使用者\]**。

4.  在 **\[搜尋使用者\]** 方塊中，輸入您要的使用者帳戶的完整或開頭部分的顯示名稱、名字、姓氏、安全性帳戶管理員 (SAM) 帳戶名稱、SIP 位址或線路統一資源識別項 (URI)，然後按一下 **\[尋找\]**。

5.  在表格中，按一下您要修改的使用者帳戶。

6.  在 **\[編輯\]** 功能表中，按一下 **\[修改\]**。

7.  在 **\[電話語音\]** 中，執行下列動作：
    
      - 若要停用使用者的音訊和視訊電話，請按一下 **\[音訊/視訊已停用\]**。
    
      - 若要啟用使用者的電腦對電腦音訊通訊，但不啟用遠端呼叫控制或 Enterprise Voice，請按一下 **\[僅限電腦對電腦\]**。針對使用者用於電腦對電腦音訊通訊的電話，指定 **\[線路 URI\]** 值。
    
      - 若要根據服務原則類別使用 Lync Server 2010 基礎結構來路由使用者電話，包括電腦對電腦音訊通訊，請按一下 **\[企業語音\]**。在 **\[線路 URI\]** 中，指定 Enterprise Voice 的電話號碼。在 **\[撥號對應表原則\]** 和 **\[語音原則\]** 中，指定使用者的適當原則。若要指定將使用者撥打的電話號碼轉譯為 E.164 格式時的正規化規則，請在 **\[位置原則\]** 中選取適當的位置設定檔。
    
      - 若要啟用遠端呼叫控制，讓使用者可以從 Lync Server 2013 控制桌上電話線，以進行電腦對電腦呼叫和電腦對電話呼叫，請按一下 **\[遠端呼叫控制\]**。在 **\[線路 URI\]** 中，指定遠端呼叫控制的電話號碼。使用者必須有桌上電話和用於電話路由的專用交換機 (PBX) 連線。

## 請參閱

#### 其他資源

[修改使用者帳戶屬性](lync-server-2013-modifying-user-account-properties.md)

