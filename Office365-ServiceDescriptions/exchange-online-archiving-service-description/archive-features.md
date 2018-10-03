---
title: Fonctionnalités d'archivage dans l'archivage Exchange Online
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/13/2018
ms.audience: ITPro
ms.topic: reference
f1_keywords:
- archive-features-in-exchange-online-archiving
ms.service: o365-administration
localization_priority: Normal
ms.custom:
- Adm_ServiceDesc
- Adm_ServiceDesc_top
ms.assetid: 38abfbd2-5aaa-444a-a431-5e71c566f3e4
description: Les sections suivantes décrivent les fonctionnalités d’archivage d’archivage Microsoft Exchange Online.
ms.openlocfilehash: 2bffa9fccb2c040fde4edcf8a5c80f3bc109bba2
ms.sourcegitcommit: d6dfbaacd56c0855e12500b38acd06be16cd1560
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/19/2018
ms.locfileid: "24035589"
---
# <a name="archive-features-in-exchange-online-archiving"></a>Fonctionnalités d'archivage dans l'archivage Exchange Online

Les sections suivantes décrivent les fonctionnalités d’archivage d’archivage Microsoft Exchange Online.
  
## <a name="archive-mailbox"></a>Boîte aux lettres d'archivage

L'Archivage Exchange Online offre aux utilisateurs des capacités d'archivage avancées avec la fonctionnalité de boîte aux lettres d'archivage. Une boîte aux lettres d'archivage est une boîte aux lettres spécialisée qui apparaît à côté des dossiers de la boîte aux lettres principale des utilisateurs dans Outlook ou Outlook Web App. Les utilisateurs peuvent accéder à l'archive de la même manière qu'ils accèdent à leur boîte aux lettres principale. En outre, ils peuvent effectuer des recherches dans leurs archives et leurs boîtes aux lettres principales.
  
Les administrateurs peuvent utiliser le Centre d'administration Exchange (CAE) ou Windows PowerShell à distance afin d'activer la fonctionnalité d'archivage pour des utilisateurs spécifiques. Pour plus d'informations, reportez-vous à la rubrique [Activer ou désactiver une boîte aux lettres d'archivage dans Exchange Online](https://go.microsoft.com/fwlink/p/?LinkId=404425).
  
> [!IMPORTANT]
>  L'utilisation de la fonction de journalisation, des règles de transport ou des règles de transfert automatique pour copier des messages dans Archivage Exchange Online à des fins d'archivage n'est pas autorisée. >  La boîte aux lettres d'archivage d'un utilisateur est destinée uniquement à cet utilisateur. Microsoft se réserve le droit de refuser l'archivage illimité dans les cas où la boîte aux lettres d'archivage d'un utilisateur sert à stocker les données d'archivage d'autres utilisateurs. 
  
### <a name="move-messages-to-exchange-online-archiving"></a>Déplacer des messages vers l'archivage Exchange Online

Les utilisateurs peuvent glisser-déplacer des messages à partir de fichiers .pst dans l'archive pour faciliter l'accès en ligne. Ils peuvent également déplacer automatiquement des éléments de messagerie de la boîte aux lettres principale vers la boîte aux lettres d'archivage à l'aide de stratégies d'archivage, de manière à réduire la taille et à améliorer les performances de la boîte aux lettres principale. Si ce comportement est différent de celui d'Exchange Hosted Archive, ce qui entraîne la création d'une copie secondaire de chaque message de l'archive, les conditions requises en matière de conservation peuvent être satisfaites dans les deux cas. Pour plus de détails sur les méthodes supplémentaires de déplacement des messages dans l'archive, reportez-vous à la rubrique [Boîtes aux lettres d'archivage dans Exchange Online](https://go.microsoft.com/fwlink/p/?LinkId=404421).
  
### <a name="import-data-to-the-archive"></a>Importer des données dans l'archive

Les utilisateurs peuvent importer des données comme suit :
  
- importer des données à partir d'un fichier .pst à l'aide de l'Assistant Importation et exportation d'Outlook ;
    
- faire glisser des messages électroniques des fichiers .PST dans l'archive ;
    
- faire glisser des messages électroniques de la boîte aux lettres principale dans l'archive ;
    
- laisser les stratégies d'archivage transférer automatiquement des messages électroniques de la boîte aux lettres principale, en fonction de l'ancienneté des messages. Pour plus d'informations, reportez-vous à la rubrique [Balises et stratégies de rétention](https://go.microsoft.com/fwlink/p/?LinkId=314153).
    
> [!NOTE]
> Les administrateurs peuvent également utiliser le service Office 365 pour importer des fichiers .pst dans les boîtes aux lettres d'archivage informatiques des utilisateurs. Pour plus d'informations, reportez-vous à la rubrique [Utiliser le chargement réseau pour importer des fichiers PST vers Office 365](https://go.microsoft.com/fwlink/p/?linkid=823074). 
  
## <a name="deleted-item-recovery"></a>Récupération d'éléments supprimés

Les utilisateurs peuvent restaurer les éléments qu'ils ont supprimés de tous les dossiers Courrier de leur archive. Quand un élément est supprimé, il est conservé dans le dossier Éléments supprimés de l'archive. Il y reste jusqu'à ce qu'il soit manuellement supprimé par l'utilisateur, ou automatiquement supprimé en raison des stratégies de rétention.
  
Une fois un élément supprimé du dossier Éléments supprimés de l'archive, il est conservé dans le dossier Éléments récupérables de l'archive pendant 14 jours supplémentaires avant d'être définitivement supprimé. Les utilisateurs peuvent récupérer ces éléments à l'aide de la fonctionnalité **Récupérer les éléments supprimés** dans Microsoft Outlook ou Outlook Web App. 
  
Si un utilisateur a purgé manuellement un élément du dossier des éléments récupérables, un administrateur peut le récupérer au cours d'une période de 14 jours à l'aide de la fonctionnalité appelée Récupération d'élément unique. Cette fonctionnalité permet aux administrateurs d'effectuer une recherche dans plusieurs boîtes aux lettres pour trouver les éléments purgés, puis d'utiliser la cmdlet Windows PowerShell  `Search-Mailbox` pour déplacer les éléments de la boîte aux lettres de découverte vers les boîtes aux lettres des utilisateurs. Pour plus d'informations, reportez-vous à la rubrique [Activation de la récupération d'élément unique pour une boîte aux lettres](https://go.microsoft.com/fwlink/p/?LinkId=314155).
  
> [!NOTE]
>  La période de récupération d'élément unique par défaut est de 14 jours, mais elle peut être personnalisée dans certains cas. >  Si un administrateur a placé la boîte aux lettres d'un utilisateur en conservation inaltérable ou en conservation pour litige, les éléments purgés sont conservés indéfiniment et la période de 14 jours ne s'applique pas. 
  
## <a name="deleted-mailbox-recovery"></a>Récupération de boîtes aux lettres supprimées

Lorsque les administrateurs suppriment des utilisateurs du serveur Exchange local, les archives de ces derniers sont également supprimées. Si les boîtes aux lettres d'archivage supprimées doivent être récupérées, l'équipe de support technique Office 365 peut effectuer cette récupération. Une archive récupérée contiendra tous les courriers qui y étaient stockés au moment de sa suppression.
  
> [!IMPORTANT]
> Les administrateurs disposent de 30 jours à partir de la suppression de la boîte aux lettres d'un utilisateur pour demander la récupération de la boîte aux lettres d'archivage. Passé ce délai de 30 jours, la boîte aux lettres d'archivage n'est plus récupérable. 
  
## <a name="mailbox-service-redundancy"></a>Redondance du service de boîte aux lettres

Boîtes aux lettres d’archivage dans l’archivage Exchange Online sont répliqués vers plusieurs copies de base de données, dans les centres de données Microsoft géographiquement dispersés, pour fournir des capacités de restauration des données en cas d’échec de l’infrastructure de messagerie. Pour les échecs à grande échelle, gestion de la continuité d’activité est déclenchée. 
  
## <a name="feature-availability"></a>Disponibilité des fonctionnalités

Pour afficher la disponibilité des fonctionnalités dans les plans Office 365, les options autonomes et les solutions locales, voir [Description du service d'archivage Exchange Online](exchange-online-archiving-service-description.md).
  