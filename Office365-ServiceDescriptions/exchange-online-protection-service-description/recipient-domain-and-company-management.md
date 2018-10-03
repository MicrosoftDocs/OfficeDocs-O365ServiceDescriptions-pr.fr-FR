---
title: Gestion des destinataires, des domaines et des entreprises
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/13/2018
ms.audience: ITPro
ms.topic: reference
f1_keywords:
- recipient-domain-and-company-management-features-in-eop
ms.service: o365-administration
localization_priority: Normal
ms.custom: Adm_ServiceDesc
ms.assetid: 10812b48-7df5-47e9-b643-dbc3c85d7de0
description: Microsoft Exchange Online Protection (EOP) offre plusieurs moyens de gestion des informations sur la société, de domaine et votre destinataire. En tant qu’administrateur, vous pouvez effectuer certaines tâches de gestion dans le centre d’administration Exchange (CAE), vérifiez autres tâches de gestion effectuées dans le centre d’administration de Microsoft Office 365.
ms.openlocfilehash: 17a87a85611dc286e3d19eaeefe04466a1ac62d0
ms.sourcegitcommit: d6dfbaacd56c0855e12500b38acd06be16cd1560
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/19/2018
ms.locfileid: "24035639"
---
# <a name="recipient-domain-and-company-management"></a>Gestion des destinataires, des domaines et des entreprises

Microsoft Exchange Online Protection (EOP) offre plusieurs moyens de gestion des informations sur la société, de domaine et votre destinataire. En tant qu’administrateur, vous pouvez effectuer certaines tâches de gestion dans le centre d’administration Exchange (CAE), vérifiez autres tâches de gestion effectuées dans le centre d’administration de Microsoft Office 365.
  
Vous recherchez des informations sur toutes les fonctionnalités EOP ? Consultez la rubrique [Description du service de protection Exchange Online](exchange-online-protection-service-description.md).
  
## <a name="mail-recipients"></a>Destinataires de messages
<a name="BKMK_mailrecipients"> </a>

Les destinataires du message sont classés en tant qu'utilisateurs ou groupes de messagerie et peuvent être gérés à l'aide de la synchronisation d'annuaires, directement dans le Centre d'administration Exchange, ou via le service Windows PowerShell à distance. Si vous gérez vos destinataires localement, vous devez synchroniser les annuaires pour que les destinataires des messages apparaissent dans le Centre d'administration Exchange. Les utilisateurs gérés uniquement dans le Centre d'administration Office 365 n'apparaissent pas dans le Centre d'administration Exchange, mais ils peuvent être ajoutés ou supprimés de l'appartenance à un groupe de rôles d'administrateur du Centre d'administration Exchange. Pour plus d'informations sur les destinataires dans EOP, consultez la rubrique [Gestion des destinataires dans Exchange Online Protection (EOP)](https://go.microsoft.com/fwlink/p/?LinkId=280011).
  
## <a name="admin-role-group-permissions"></a>Autorisations de groupe de rôles d'administrateur
<a name="BKMK_adminrolegrouppermissions"> </a>

Dans EOP, vous pouvez configurer uniquement des rôles d'administrateur. Le Centre d'administration Exchange vous permet d'ajouter directement des utilisateurs à des groupes de rôles d'administrateur par défaut ou d'en supprimer. Aucune personnalisation RBAC n'est disponible. Pour plus d'informations, consultez la rubrique [Gérer les autorisations de groupe de rôles d'administrateur dans EOP](https://go.microsoft.com/fwlink/p/?LinkId=282238).
  
## <a name="domain-management"></a>Gestion de domaines
<a name="BKMK_domainmanagement"> </a>

Les domaines gérés sont des domaines protégés par EOP. Le Centre d'administration Exchange permet d'afficher les domaines gérés et de modifier les types de domaines. L'approvisionnement et la gestion des domaines s'effectuent dans le Centre d'administration Office 365 et les modifications apparaissent dans le Centre d'administration Exchange. Pour plus d'informations, consultez la rubrique [Gérer des domaines acceptés dans EOP](https://go.microsoft.com/fwlink/p/?LinkId=282239).
  
## <a name="match-subdomains"></a>Mise en correspondance des sous-domaines
<a name="BKMK_EOP_Match_Subdomains"> </a>

Dans EOP, vous pouvez activer le flux de messagerie pour les sous-domaines d'un domaine géré. Pour plus d'informations, consultez la rubrique [Activer le flux de messagerie pour les sous-domaines dans EOP](https://go.microsoft.com/fwlink/p/?LinkId=397213). 
  
## <a name="directory-based-edge-blocking-dbeb"></a>Blocage du périmètre basé sur l'annuaire (DBEB)
<a name="BKMK_DBEB"> </a>

La fonctionnalité de blocage du périmètre basé sur l'annuaire vous permet de rejeter les messages pour les destinataires non valides sur le périmètre du réseau de service. La fonctionnalité de blocage du périmètre basé sur l'annuaire (DBEB) permet aux administrateurs d'ajouter des destinataires à extension messagerie à Office 365 et de bloquer tous les messages envoyés à des adresses de messagerie qui ne sont pas présentes dans Office 365. Si un message est envoyé à une adresse de messagerie valide présente dans Office 365, celui-ci continue à travers le reste des couches de filtrage de services (anti-programme malveillant, anti-courrier indésirable, règles de transport). Si l'adresse n'est pas présente, le service bloque le message avant même le filtrage, et une notification d'échec de remise (NDR) est envoyée à l'expéditeur pour l'informer que son message n'a pas été remis. 
  
L'activation de DBEB nécessite une configuration utilisateur et une configuration de domaine. Pour plus d'informations, consultez la rubrique [Utiliser le blocage du périmètre basé sur l'annuaire pour rejeter les messages envoyés à des destinataires non valides](https://go.microsoft.com/fwlink/p/?LinkId=390676).
  
## <a name="feature-availability"></a>Disponibilité des fonctionnalités
<a name="BKMK_DBEB"> </a>

Pour afficher la disponibilité des fonctionnalités dans les plans Office 365, les options autonomes et les solutions locales, voir [Description du service de protection Exchange Online](exchange-online-protection-service-description.md).
  
