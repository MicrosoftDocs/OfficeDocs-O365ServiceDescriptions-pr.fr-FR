---
title: Description du service d'archivage Exchange Online
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/13/2018
ms.audience: ITPro
ms.topic: reference
f1_keywords:
- exchange-online-archiving-service-description
ms.service: o365-administration
localization_priority: Normal
ms.custom:
- Adm_ServiceDesc_top
- Adm_ServiceDesc
ms.assetid: 21ebd4bb-7d88-489f-a8aa-376e2536900c
description: Archivage Microsoft Exchange Online est une Microsoft Office 365 en nuage, d’archivage solution d’entreprise pour les organisations qui ont déployé Microsoft Exchange Server 2013, Microsoft Exchange Server 2010 (SP2 et versions ultérieures), ou vous abonner à certains Exchange Online ou Office 365 plans. L’archivage Exchange Online aide les organisations avec leurs d’archivage, la conformité aux exigences réglementaires, et eDiscovery défis lors de la simplification de l’infrastructure locale et réduction des coûts et accélération des charges de l’informatique.
ms.openlocfilehash: d88d336f0e5b30a245b6c90c7cc488ca6d5dfc54
ms.sourcegitcommit: d6dfbaacd56c0855e12500b38acd06be16cd1560
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/19/2018
ms.locfileid: "24035522"
---
# <a name="exchange-online-archiving-service-description"></a>Description du service d'archivage Exchange Online

Archivage Microsoft Exchange Online est une Microsoft Office 365 en nuage, d’archivage solution d’entreprise pour les organisations qui ont déployé Microsoft Exchange Server 2013, Microsoft Exchange Server 2010 (SP2 et versions ultérieures), ou vous abonner à certains Exchange Online ou Office 365 plans. L’archivage Exchange Online aide les organisations avec leurs d’archivage, la conformité aux exigences réglementaires, et eDiscovery défis lors de la simplification de l’infrastructure locale et réduction des coûts et accélération des charges de l’informatique.
  
En tant que service en ligne Microsoft Office 365, l'Archivage Exchange Online est conçu pour aider à répondre aux besoins grandissants de sécurité, de fiabilité et de productivité des utilisateurs. Pour plus d'informations sur Office 365, notamment sur les fonctionnalités communes à tous les services en ligne Office 365, consultez la rubrique [Description du service de plateforme Office 365](../office-365-platform-service-description/office-365-platform-service-description.md).
  
Pour acheter la solution Archivage Exchange Online, consultez la page [Archivage Exchange Online](https://go.microsoft.com/fwlink/p/?LinkId=314176).
  
Pour comparer les fonctionnalités des différents plans, voir [Comparer toutes les offres Office 365 pour les entreprises](http://go.microsoft.com/fwlink/?LinkID=799177&amp;clcid=0x409).
  
> [!TIP]
> Vous pouvez exporter, enregistrer et imprimer des pages dans les descriptions du service Office 365. Découvrez comment [exporter plusieurs pages](https://go.microsoft.com/fwlink/?LinkId=403349). 
  
## <a name="exchange-online-archiving-plans"></a>Plans d'archivage Exchange Online
<a name="bkmk_EOA_Plans"> </a>

L'Archivage Exchange Online est disponible dans les plans suivants.
  
|**Plan**|**Description**|
|:-----|:-----|
|**Archivage Exchange Online pour Exchange Server** <br/> |Archive en nuage pour les utilisateurs disposant de boîtes aux lettres principales dans Exchange Server 2013 ou Exchange 2010 (SP2 ou version ultérieure).  <br/> Si vous souhaitez ajouter une archive basée sur le cloud à une boîte aux lettres principale située sur un serveur Exchange local, vous devez configurer un déploiement hybride. Pour plus d'informations sur les déploiements hybrides, voir [Déploiements hybrides Exchange Server](https://technet.microsoft.com/library/jj200581%28v=exchg.150%29.aspx).  <br/> |
|**Archivage Exchange Online pour Exchange Server (via Enterprise CAL Suite).** <br/> |Archive en nuage pour les utilisateurs disposant de boîtes aux lettres principales dans Exchange Server 2013 ou Exchange 2010 (SP2 ou version ultérieure). Pour en savoir plus, consultez les [informations relatives aux licences Core CAL Suite et Enterprise CAL Suite](https://go.microsoft.com/fwlink/p/?LinkId=314160).  <br/> |
|**Archivage Exchange Online pour Exchange Online** <br/> | Archive en nuage et archive permanente comme module complémentaire pour les plans suivants : <sup>1, 2</sup>,  <br/>  Exchange Online Plan 1  <br/>  Exchange Online Kiosk  <br/>  Office 365 Business Essentials  <br/>  Office 365 Business Premium  <br/>  Office 365 Entreprise E1  <br/>  Office 365 Entreprise F1  <br/> > [!NOTE]> Les plans suivants incluent l’archivage déjà et ne nécessitent pas l’archivage Exchange Online en tant que composant additionnel : > Office 365 éducation A1 > Office 365 éducation A3 > Office 365 éducation A5 > Office 365 entreprise E3 > Office 365 entreprise E5 > Exchan GE Online Plan 2 > Pour plus d’informations sur les fonctionnalités d’archivage de boîtes aux lettres Exchange Online, consultez [archivage de boîtes aux lettres dans Exchange Online](https://go.microsoft.com/fwlink/p/?LinkId=404421).           |
   
> [!NOTE]
> <sup>1</sup> Le déploiement hybride n'est pas requis pour les organisations en nuage uniquement sans boîte aux lettres située sur un serveur Exchange local. Toutefois, s'il existe des boîtes aux lettres locales, le déploiement hybride est requis. > <sup>2</sup> Les plans Exchange Online Plan 1 et Office 365 Business ont une [limite de taille pour les boîtes aux lettres et les archives](https://go.microsoft.com/fwlink/?LinkId=330039). L'Archivage Exchange Online pour le module complémentaire Exchange Online ajoute une archive informatique illimitée et une [Conservation inaltérable et conservation pour litige](compliance-and-security-features.md#in-place-hold-and-litigation-hold). 
  
Vous recherchez des informations sur tous les plans Office 365 ? Office 365 est disponible dans le cadre de différents plans destinés à répondre au mieux aux besoins de votre organisation. Pour plus d'informations sur les plans, y compris les options de plan autonome, et sur le passage d'un plan à un autre, consultez la rubrique [Options de plan Office 365](../office-365-platform-service-description/office-365-plan-options.md).
  
## <a name="requirements"></a>Configuration requise
<a name="bkmk_EOA_Plans"> </a>

Afin d'utiliser l'Archivage Exchange Online pour Exchange Server, les boîtes aux lettres des utilisateurs doivent résider sur Exchange Server 2013 ou Exchange Server 2010 (SP2 ou ultérieur).
  
### <a name="federated-identity-and-single-sign-on"></a>Identité fédérée et authentification unique

Les administrateurs peuvent utiliser une approche d’authentification unique pour l’authentification Office 365 avec Active Directory sur site. Pour ce faire, ils peuvent configurer les services ADFS (Active Directory Federation Services) sur site (service Microsoft Windows Server ® 2008) à fédérer avec Microsoft Federation Gateway. Une fois les services ADFS (Active Directory Federation Services) configurés, tous les utilisateurs d’Office 365 dont l’identité est fondée sur le domaine fédéré peuvent utiliser leur session d’entreprise existante pour s’authentifier automatiquement dans Office 365.
  
### <a name="user-subscriptions"></a>Abonnements utilisateur

Chaque utilisateur qui accède au service d'Archivage Exchange Online doit posséder un abonnement d'Archivage Exchange Online. Chaque abonnement d'archivage de courrier électronique peut être utilisé uniquement pour le stockage des données de messagerie d'un utilisateur.
  
## <a name="unlimited-archive-storage-quota"></a>Quota de stockage d'archive illimité
<a name="bkmk_EOA_Plans"> </a>

 La fonctionnalité d'archivage illimité d'Office 365 (appelée archivage à extension automatique) fournit un espace illimité de stockage dans les boîtes aux lettres d'archivage. Au départ, chaque abonné Archivage Exchange Online reçoit 100 Go de stockage dans la boîte aux lettres d'archivage. Lorsque l'archivage à extension automatique est activé, un espace de stockage supplémentaire est ajouté automatiquement lorsque la capacité de stockage de 100 Go est atteinte. Pour plus d'informations, reportez-vous à la rubrique [Présentation de l'archivage illimité dans Office 365](https://go.microsoft.com/fwlink/?linkid=844060). Pour plus de détails sur la disponibilité, consultez la [feuille de route d'Office 365](http://go.microsoft.com/fwlink/?LinkId=509914). 
  
> [!IMPORTANT]
> Les administrateurs ne peuvent pas ajuster le quota de stockage. 
  
> [!IMPORTANT]
> L'utilisation de la fonction de journalisation, des règles de transport ou des règles de transfert automatique pour copier des messages dans Archivage Exchange Online à des fins d'archivage n'est pas autorisée. La boîte aux lettres d'archivage d'un utilisateur est destinée uniquement à cet utilisateur. Microsoft se réserve le droit de refuser l'archivage illimité dans les cas où la boîte aux lettres d'archivage d'un utilisateur sert à stocker les données d'archivage d'autres utilisateurs. 
  
## <a name="feature-availability-across-exchange-online-archiving-plans"></a>Disponibilité des fonctionnalités pour les différents plans d'archivage Exchange Online
<a name="bkmk_EOA_Plans"> </a>

||||
|:-----|:-----|:-----|
|**Fonctionnalité** <br/> |**Archivage Exchange Online pour Exchange Server<sup>1</sup>**          <br/> |**Archivage Exchange Online pour Exchange Online<sup>2</sup>** <br/> |
|**[Fonctionnalités d'archivage dans l'archivage Exchange Online](archive-features.md)** <br/> |||
|Boîte aux lettres d'archivage  <br/> |Oui  <br/> |Oui  <br/> |
|Déplacer les messages à l'aide de la stratégie d'archivage  <br/> |Oui  <br/> |Oui  <br/> |
|Importer des données dans l'archive  <br/> |Oui  <br/> |Oui  <br/> |
|Récupération d'éléments supprimés  <br/> |Oui  <br/> |Oui  <br/> |
|Récupération de boîtes aux lettres supprimées  <br/> |Oui  <br/> |Oui  <br/> |
|Sauvegarde de boîtes aux lettres  <br/> |Oui  <br/> |Oui  <br/> |
|**[Fonctionnalités client dans l'archivage Exchange Online](client-features.md)** <br/> |||
|Outlook<sup>3</sup> <br/> |Oui  <br/> |Oui  <br/> |
|Outlook Web App  <br/> |Oui  <br/> |Oui  <br/> |
|**[Fonctionnalités de conformité et de sécurité dans l'archivage Exchange Online](compliance-and-security-features.md)** <br/> |||
|Stratégies de rétention  <br/> |Oui  <br/> |Oui  <br/> |
|Conservation inaltérable et conservation pour litige<sup>6</sup> <br/> |Oui  <br/> |Oui  <br/> |
|Découverte électronique locale  <br/> |Oui  <br/> |Oui  <br/> |
|Chiffrement entre serveurs sur site et archivage Exchange Online  <br/> |Oui  <br/> |Oui  <br/> |
|Chiffrement entre clients et archivage Exchange Online  <br/> |Oui  <br/> |Oui  <br/> |
|Chiffrement : S/MIME et PGP  <br/> |Oui  <br/> |Oui  <br/> |
|IRM avec Azure Information Protection  <br/> |Non  <br/> |Aucun<sup>4</sup> <br/> |
|IRM via Windows Server AD RMS  <br/> |Oui<sup>5</sup> <br/> |Oui<sup>5</sup> <br/> |
|Audit  <br/> |Oui  <br/> |Oui  <br/> |
   

> <sup>1</sup> Les boîtes aux lettres utilisateur doivent résider sur Exchange 2010 SP2 ou version ultérieure.
 <br/><sup>2</sup> une Archive In-Place uniquement utilisable pour archiver des messages pour un utilisateur unique ou d’une entité pour laquelle une licence a été appliquée. À l’aide d’une Archive In-Place comme moyen pour stocker le courrier provenant de plusieurs utilisateurs ou des entités est interdite. Par exemple, les administrateurs informatiques ne peut pas créer des boîtes aux lettres partagées et des utilisateurs de copier (via le champ Cc ou Cci, ou une règle de transport) une boîte aux lettres partagée dans le but explicit de l’archivage. <br/> <sup>3</sup> pour une liste des versions prises en charge de Microsoft Outlook, voir [Fonctionnalités Client dans l’archivage Exchange Online](client-features.md). 
 <br/><sup>4</sup> azure la Protection des informations n’est pas incluse, mais peut être achetée en tant que module complémentaire séparé et activera les fonctionnalités d’Information Rights Management (IRM) pris en charge. Certaines fonctionnalités de Protection des informations Azure requièrent un abonnement à Office 365 ProPlus, qui n’est pas inclus avec Office 365 entreprise Essentials, Office 365 entreprise Premium, Office 365 entreprise E1, Office 365 éducation ou Office 365 entreprise F1. <br/><sup>5</sup> Windows Server AD RMS est un serveur local qui doit être acheté et géré séparément afin d'activer les fonctionnalités IRM prises en charge. 
 <br/><sup>6</sup> Lorsque vous placez une boîte aux lettres en conservation inaltérable ou en conservation pour litige, la conservation porte à la fois sur la boîte aux lettres d'archivage et la boîte aux lettres principale. 