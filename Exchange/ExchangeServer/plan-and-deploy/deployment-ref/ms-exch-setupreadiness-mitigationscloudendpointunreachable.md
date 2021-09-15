---
ms.localizationpriority: medium
monikerRange: exchserver-2016 || exchserver-2019
description:  Mitigations Cloud endpoint is not reachable
ms.topic: reference
author: joannehendrickson
ms.custom:
- ms-exch-setupreadiness-KB2999226NotInstalled
ms.author: jhendr
ms.reviewer: 
title: Mitigations Cloud endpoint is not reachable
ms.collection: exchange-server
f1.keywords:
- CSH
audience: ITPro
ms.prod: exchange-server-it-pro
manager: serdars
---
#  Mitigations loud endpoint is not reachable

::: moniker range="exchserver-2016"

Microsoft Exchange Server 2016 setup displayed this warning because the setup failed to connect to the Mitigation Service Cloud endpoint from the local computer. 

Exchange 2016 (CU22) setup installs the Exchange Emergency Mitigation (EM) Service. The EM Service checks for available mitigations every hour before downloading and applying them. 

::: moniker-end

::: moniker range="exchserver-2019"
Microsoft Exchange Server 2019 setup displayed this warning because the setup failed to connect to the Mitigation Service Cloud endpoint from the local computer. 

Exchange 2019 (CU11) setup installs the Exchange Emergency Mitigation (EM) Service. The EM Service checks for available mitigations every hour before downloading and applying them. 

::: moniker-end

The functionality to check and download mitigations needs outbound connectivity to the Mitigation Service Cloud endpoint. Without this connectivity, the EM service can’t function, which can pose a security risk. We recommend enabling connectivity with the Mitigation Service Cloud endpoint from the computer on which Exchange Server is installed for the EM service to function correctly. 


|Required|Address|Port|
|:-----|:-----|:-----|:-----|
|Yes|officeclient.microsoft.com/*|443|

**Having problems?** Ask for help in the Exchange forums. Visit the forums at: [Exchange Server](https://social.technet.microsoft.com/forums/office/home?category=exchangeserver)