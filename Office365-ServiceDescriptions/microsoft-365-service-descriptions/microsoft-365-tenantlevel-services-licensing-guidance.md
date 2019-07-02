---
title: Conseils pour la gestion des licences des services de niveau client Microsoft 365
ms.author: sharik
author: skjerland
manager: mnirkhe
audience: ITPro
ms.topic: reference
f1_keywords:
- office-online-service-description
ms.service: o365-administration
localization_priority: Normal
ms.custom: Adm_ServiceDesc
description: Cet article fournit des conseils en matière de licences pour les services de niveau client Microsoft 365 afin d’éviter une interruption potentielle des services due à un accès sans licence.
ms.openlocfilehash: dea49f7c6ea3a0082968335586e146a33d4a76cc
ms.sourcegitcommit: 983c4e2b50177883d9369f12b43e09d51e1e5f28
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/01/2019
ms.locfileid: "35411459"
---
# <a name="microsoft-365-tenant-level-services-licensing-guidance"></a>Conseils pour la gestion des licences des services de niveau client Microsoft 365

Pour les besoins de cet article, un service au niveau du client est un service en&mdash;ligne qui, lorsqu’il est acheté pour n’importe quel utilisateur dans le client (autonome ou en tant que&mdash;partie de plans Office 365 ou Microsoft 365) est activé partiellement ou intégralement pour tous les utilisateurs du client. Bien que certains utilisateurs sans licence puissent techniquement être en mesure d’accéder au service, une licence est requise pour tous les utilisateurs que vous envisagez de bénéficier du service.

> [!NOTE]
> Certains services de client ne sont actuellement pas en mesure de limiter les avantages à des utilisateurs spécifiques. Les efforts doivent être pris pour limiter les avantages du service aux utilisateurs titulaires d’une licence. Cela permettra d’éviter une interruption potentielle des services pour votre organisation une fois que les fonctionnalités de ciblage sont disponibles.

## <a name="azure-active-directory-identity-protection"></a>Azure Active Directory Identity Protection

La protection des identités Azure Active Directory (AADIP) est une fonctionnalité du plan Azure Active Directory Premium P2 qui vous permet de détecter les vulnérabilités potentielles affectant les identités de votre organisation, de configurer des réponses automatiques pour détecter des problèmes suspects. actions liées aux identités de votre organisation et enquête sur les incidents suspects et mesures appropriées pour les résoudre.

### <a name="which-users-benefit-from-the-service"></a>Quels sont les utilisateurs qui bénéficient du service?

Les utilisateurs sous licence d’Enterprise Mobility + Security E5, Microsoft 365 E5, Microsoft 365 E5 sécurité et Azure Active Directory Premium plan 2 peuvent bénéficier de AADIP.

### <a name="how-do-users-benefit-from-the-service"></a>Comment les utilisateurs bénéficient-ils du service?

Les analystes et les professionnels de la sécurité de SECOPS bénéficient d’un affichage consolidé des utilisateurs avec indicateur et des événements de risque basés sur des algorithmes d’apprentissage automatique. Les utilisateurs finaux bénéficient de la protection automatique offerte par un accès conditionnel basé sur des risques et la sécurité améliorée offerte par les vulnérabilités.

### <a name="how-is-the-service-provisioneddeployed"></a>Comment le service est-il configuré/déployé?

Par défaut, les fonctionnalités AADIP sont activées au niveau du client pour tous les utilisateurs au sein du client. Pour plus d’informations sur la configuration de AADIP, consultez la rubrique activation de la [protection des identités Azure Active Directory](https://docs.microsoft.com/azure/active-directory/identity-protection/enable).

### <a name="how-can-the-service-be-applied-only-to-users-in-the-tenant-who-are-licensed-for-the-service"></a>Comment le service peut-il être appliqué uniquement aux utilisateurs du client qui sont titulaires d’une licence pour ce service?

Les administrateurs peuvent définir l’étendue AADIP en affectant des stratégies de risque qui définissent le niveau des réinitialisations de mot de passe et autorisent l’accès aux utilisateurs sous licence uniquement. Pour obtenir des instructions sur l’étendue des déploiements AADIP, consultez [la rubrique Configure the sign-in Risk Policy](https://docs.microsoft.com/azure/active-directory/identity-protection/howto-sign-in-risk-policy).

## <a name="azure-advanced-threat-protection"></a>Protection avancée contre les menaces

La protection avancée contre les menaces (ATP) est un service Cloud qui permet de protéger les environnements hybrides d’entreprise contre plusieurs types de menaces informatiques ciblées avancées et de menaces Insiders.

### <a name="which-users-benefit-from-the-service"></a>Quels sont les utilisateurs qui bénéficient du service?

Les utilisateurs sous licence de Enterprise Mobility + Security E5, Microsoft 365 E5, Microsoft 365 E5 sécurité et Azure Advanced Threat Protection pour les utilisateurs peuvent bénéficier d’Azure ATP.

### <a name="how-do-users-benefit-from-the-service"></a>Comment les utilisateurs bénéficient-ils du service?

Les analystes et les professionnels de la sécurité d’SecOp bénéficient de la capacité d’Azure ATP à détecter et à examiner les menaces avancées, les identités compromises et les actions malveillantes. Les utilisateurs finaux bénéficient de leurs données surveillées par Azure ATP.

### <a name="how-is-the-service-provisioneddeployed"></a>Comment le service est-il configuré/déployé?

Par défaut, les fonctionnalités Azure ATP sont activées au niveau du client pour tous les utilisateurs au sein du client. Pour plus d’informations sur la configuration d’Azure ATP, voir [Create Your Azure ATP instance](https://docs.microsoft.com/azure-advanced-threat-protection/install-atp-step1).

### <a name="how-can-the-service-be-applied-only-to-users-in-the-tenant-who-are-licensed-for-the-service"></a>Comment le service peut-il être appliqué uniquement aux utilisateurs du client qui sont titulaires d’une licence pour ce service?

Microsoft ne s’engage pas à fournir des fonctionnalités de détection des menaces pour les utilisateurs qui ne sont pas titulaires d’une licence. Au fil du temps, les vérifications de licence ou les outils ciblés seront ajoutés à Azure ATP pour s’assurer que la fonctionnalité ATP Azure s’applique uniquement aux utilisateurs sous licence.

## <a name="azure-information-protection"></a>Azure Information Protection

Azure information protection (AIP) aide les organisations à découvrir, classer, étiqueter et protéger des documents et e-mails sensibles. Les administrateurs peuvent définir des règles et des conditions pour appliquer les étiquettes automatiquement, les utilisateurs peuvent appliquer des étiquettes manuellement ou une combinaison des&mdash;deux peuvent être utilisées lorsque les utilisateurs reçoivent des recommandations sur l’application d’étiquettes.

### <a name="which-users-benefit-from-the-service"></a>Quels sont les utilisateurs qui bénéficient du service?

Les utilisateurs titulaires d’une licence Microsoft 365 F1, Microsoft 365 E3 et AIP plan 1 peuvent bénéficier de l’AIP plan 1. Les utilisateurs titulaires d’une licence Microsoft 365 E5, Microsoft 365 E5 conformité et le plan administrative 2 peuvent bénéficier de l’AIP plan 2.

### <a name="how-do-users-benefit-from-the-service"></a>Comment les utilisateurs bénéficient-ils du service?

La fonctionnalité de scanneur AIP classe, étiquette et protège automatiquement les fichiers qui se trouvent dans les référentiels de fichiers locaux.

### <a name="how-is-the-service-provisioneddeployed"></a>Comment le service est-il configuré/déployé?

Par défaut, les fonctionnalités AIP sont activées au niveau du client pour tous les utilisateurs au sein du client. Pour plus d’informations sur la configuration des stratégies AIP pour les utilisateurs sous licence, consultez la rubrique activation de la [gestion des droits Azure](https://docs.microsoft.com/azure/information-protection/activate-service).

### <a name="how-can-the-service-be-applied-only-to-users-in-the-tenant-who-are-licensed-for-the-service"></a>Comment le service peut-il être appliqué uniquement aux utilisateurs du client qui sont titulaires d’une licence pour ce service?

Les stratégies de fonctionnalité AIP (à l’exception de la fonctionnalité scanneur) peuvent être étendues à des groupes ou à des utilisateurs spécifiques; les registres peuvent être modifiés pour empêcher les utilisateurs sans licence d’exécuter des fonctionnalités de classification ou d’étiquetage AIP. Pour obtenir des instructions sur la façon d’étendre les déploiements AIP, consultez [la rubrique Configuration de la stratégie Azure information protection](https://docs.microsoft.com/azure/information-protection/configure-policy).

Pour la fonctionnalité de scanneur AIP, Microsoft ne s’engage pas à fournir des fonctionnalités de classification, d’étiquetage ou de protection des fichiers aux utilisateurs qui ne sont pas titulaires d’une licence. Au fil du temps, les vérifications de licence ou les outils ciblés seront ajoutés à AIP pour s’assurer que la fonctionnalité de scanneur peut être attribuée aux utilisateurs titulaires d’une licence.

## <a name="office-365-advanced-threat-protection"></a>Office 365-Protection avancée contre les menaces

La protection avancée contre les menaces (ATP) permet de protéger les organisations contre des attaques sophistiquées telles que le hameçonnage et les programmes malveillants de jour zéro jour. Elle fournit également des informations utiles en mettant en corrélation les signaux provenant d’un large éventail de données pour identifier, hiérarchiser et fournir des recommandations sur la façon de résoudre les menaces potentielles.

### <a name="which-users-benefit-from-the-service"></a>Quels sont les utilisateurs qui bénéficient du service?

Les utilisateurs titulaires d’une licence d’Office 365 E5, Microsoft 365 E5, Microsoft 365 E5 sécurité, Microsoft 365 Business et Office 365 ATP (plans 1 et 2) peuvent bénéficier de la protection avancée contre les menaces.

### <a name="how-do-users-benefit-from-the-service"></a>Comment les utilisateurs bénéficient-ils du service?

ATP protège les utilisateurs contre les attaques sophistiquées telles que le hameçonnage et les programmes malveillants de jour zéro jour. Pour obtenir la liste complète des services fournis dans plan 1 et plan 2, consultez la rubrique [Office 365 Advanced Threat Protection](https://products.office.com/exchange/advance-threat-protection).

### <a name="how-is-the-service-provisioneddeployed"></a>Comment le service est-il configuré/déployé?

Par défaut, les fonctionnalités ATP sont activées au niveau du client pour tous les utilisateurs au sein du client. Pour plus d’informations sur la configuration des stratégies ATP pour les utilisateurs sous licence, consultez la rubrique [Office 365 Advanced Threat Protection](https://docs.microsoft.com/office365/securitycompliance/office-365-atp).

### <a name="how-can-the-service-be-applied-only-to-users-in-the-tenant-who-are-licensed-for-the-service"></a>Comment le service peut-il être appliqué uniquement aux utilisateurs du client qui sont titulaires d’une licence pour ce service?

À l’étendue ATP, suivez les stratégies de déploiement des pièces jointes fiables et des liens fiables:

  - Pour plus d’informations sur la configuration des liens fiables pour les utilisateurs sous licence, consultez la rubrique [set up Office 365 ATP Safe Links Policies](https://docs.microsoft.com/office365/securitycompliance/set-up-atp-safe-links-policies).

  - Pour plus d’informations sur la configuration des pièces jointes fiables pour les utilisateurs sous licence, consultez la rubrique [set up Office 365 ATP Safe Attachments Policies](https://docs.microsoft.com/office365/securitycompliance/set-up-atp-safe-attachments-policies).

## <a name="office-365-cloud-app-security"></a>Sécurité de l’application cloud Office 365

Office 365 Cloud App Security (OCAS) est un sous-ensemble de la sécurité des applications Cloud de Microsoft, avec des fonctionnalités limitées à Office 365 et sans sécurité supplémentaire pour les applications Cloud tierces et les services IaaS.

OCAS donne aux organisations une visibilité sur leurs applications et services de Cloud de productivité, fournit des analyses sophistiquées pour identifier et combattre les menaces informatiques,&mdash;et leur permet de contrôler la façon dont les données circulent dans Office 365.

Pour comparer les fonctionnalités, consultez la rubrique [differences between Microsoft Cloud App Security and Office 365 Cloud App Security](https://docs.microsoft.com/cloud-app-security/editions-cloud-app-security-o365).

### <a name="which-users-benefit-from-the-service"></a>Quels sont les utilisateurs qui bénéficient du service?

Les utilisateurs sous licence d’Office 365 E5 peuvent tirer parti de OCAS.

Pour plus d’informations, reportez-vous à la feuille de données [Microsoft Cloud App Security Licensing](http://www.aka.ms/mcaslicensing).

### <a name="how-do-users-benefit-from-the-service"></a>Comment les utilisateurs bénéficient-ils du service?

OCAS les identifie, fournit une protection contre les menaces dans Office 365 et peut contrôler les applications qui ont l’autorisation d’accéder aux données Office 365.

### <a name="how-is-the-service-provisioneddeployed"></a>Comment le service est-il configuré/déployé?

Par défaut, les fonctionnalités OCAS sont activées au niveau du client pour tous les utilisateurs au sein du client.

Pour plus d’informations sur la configuration du service, voir [Basic Setup for Cloud App Security](https://docs.microsoft.com/cloud-app-security/general-setup).

### <a name="how-can-the-service-be-applied-only-to-users-in-the-tenant-who-are-licensed-for-the-service"></a>Comment le service peut-il être appliqué uniquement aux utilisateurs du client qui sont titulaires d’une licence pour ce service?

Les administrateurs peuvent étendre les déploiements OCAS pour appliquer la manière dont certaines applications sont consultées et limiter les groupes d’utilisateurs surveillés par la sécurité des applications Cloud d’Office 365. Pour plus d’informations, reportez-vous à la rubrique [déploiement étendu](https://docs.microsoft.com/cloud-app-security/scoped-deployment).

## <a name="microsoft-cloud-app-security"></a>Microsoft Cloud App Security

Microsoft Cloud App Security (MCAS) est une solution CASB (Cloud Access Security Broker) qui donne aux organisations une visibilité sur leurs applications et services Cloud, fournit des analyses sophistiquées pour identifier et combattre les menaces informatiques, et leur permet de contrôler la façon dont les données se&mdash;déplace dans n’importe quelle application Cloud.

### <a name="which-users-benefit-from-the-service"></a>Quels sont les utilisateurs qui bénéficient du service?

Les utilisateurs titulaires d’une licence MCAS, Enterprise Mobility + Security E5, Microsoft 365 E5 et Microsoft 365 E5 Security peuvent bénéficier de MCAS.

Les utilisateurs sous licence d’Azure AD P1 peuvent bénéficier des fonctionnalités de découverte dans MCAS.

Pour bénéficier des fonctionnalités de [contrôle d’application d’accès conditionnel](https://docs.microsoft.com/cloud-app-security/proxy-intro-aad) dans MCAS, les utilisateurs doivent également être titulaires d’une licence pour Azure Active Directory P1, inclus dans Enterprise Mobility + Security E3, Enterprise Mobility + Security E5, Microsoft 365 E3, Microsoft 365 E5 et Microsoft 365 E5 sécurité.

Pour bénéficier de l' [étiquetage automatique](https://docs.microsoft.com/cloud-app-security/data-protection-policies), les utilisateurs doivent disposer d’une licence pour Azure information protection P2, inclus dans Enterprise Mobility + Security E5, Microsoft 365 E5 et Microsoft 365 E5 conformité.

Pour plus d’informations, reportez-vous à la feuille de données [Microsoft Cloud App Security Licensing](http://www.aka.ms/mcaslicensing).

### <a name="how-do-users-benefit-from-the-service"></a>Comment les utilisateurs bénéficient-ils du service?

MCAS identifie et évalue l’ombre, fournit une protection contre les menaces entre les applications Cloud First et tierces, et protège les informations des applications Cloud de première et tierces.

### <a name="how-is-the-service-provisioneddeployed"></a>Comment le service est-il configuré/déployé?

Par défaut, les fonctionnalités MCAS sont activées au niveau du client pour tous les utilisateurs au sein du client.

Pour plus d’informations sur la configuration des stratégies de sécurité de l’application Cloud Microsoft pour les utilisateurs titulaires d’une licence, voir [Microsoft Cloud App Security Overview](https://docs.microsoft.com/cloud-app-security/what-is-cloud-app-security).

### <a name="how-can-the-service-be-applied-only-to-users-in-the-tenant-who-are-licensed-for-the-service"></a>Comment le service peut-il être appliqué uniquement aux utilisateurs du client qui sont titulaires d’une licence pour ce service?

Les administrateurs peuvent étendre les déploiements MCAS aux utilisateurs titulaires d’une licence à l’aide des fonctionnalités de déploiement étendues disponibles dans le service. Pour plus d’informations, reportez-vous à la rubrique [déploiement étendu](https://docs.microsoft.com/cloud-app-security/scoped-deployment).

## <a name="office-365-advanced-data-governance"></a>Gouvernance des données avancée Office 365

Advanced Data Governance (ADG) aide les organisations à répondre aux exigences de gouvernance des informations avec des stratégies pour activer la rétention et la suppression. ADG permet aux organisations d’étiqueter automatiquement le contenu en fonction du type d’informations sensibles et d’appliquer des stratégies de gouvernance à ce contenu.

### <a name="which-users-benefit-from-the-service"></a>Quels sont les utilisateurs qui bénéficient du service?

Les utilisateurs titulaires d’une licence Office 365 E5, Microsoft 365 E5, conformité à la réglementation Microsoft 365 E5 et Office 365 Advanced Compliance peuvent tirer parti de ADG.

### <a name="how-do-users-benefit-from-the-service"></a>Comment les utilisateurs bénéficient-ils du service?

ADG permet aux utilisateurs d’appliquer des étiquettes à des données spécifiques afin de maintenir des stratégies spécifiques, d’étiqueter automatiquement le contenu sous la forme d’un enregistrement et de gérer le processus complet des enregistrements à partir de la déclaration jusqu’à la suppression.

### <a name="how-is-the-service-provisioneddeployed"></a>Comment le service est-il configuré/déployé?

Par défaut, les fonctionnalités ADG sont activées au niveau du client pour tous les utilisateurs au sein du client. Pour plus d’informations sur la configuration d’ADG pour l’application de l’étiquetage automatique et des stratégies pour les utilisateurs sous licence, consultez la rubrique [vue d’ensemble des étiquettes de](https://docs.microsoft.com/office365/securitycompliance/labels)rétention.

### <a name="how-can-the-service-be-applied-only-to-users-in-the-tenant-who-are-licensed-for-the-service"></a>Comment le service peut-il être appliqué uniquement aux utilisateurs du client qui sont titulaires d’une licence pour ce service?

Les stratégies de rétention ADG peuvent être appliquées aux utilisateurs titulaires d’une licence dans des emplacements spécifiques (sites d’équipe, sites de groupe, etc.) par le biais de la classification automatique. Pour obtenir des instructions sur l’application des stratégies de rétention ADG, consultez [la rubrique application d’une stratégie de rétention à une organisation ou à des emplacements spécifiques](https://docs.microsoft.com/office365/securitycompliance/retention-policies#applying-a-retention-policy-to-an-entire-organization-or-specific-locations).

## <a name="office-365-advanced-ediscovery"></a>eDiscovery (découverte électronique) avancée Office 365

Advanced eDiscovery fournit des solutions d’enquête et de découverte électronique pour les services informatiques et juridiques au sein des organisations afin d’identifier, de collecter, de conserver, de réduire et de consulter le contenu lié à une enquête ou un litige avant l’exportation en dehors d’Office 365 Configuration.

### <a name="which-users-benefit-from-the-service"></a>Quels sont les utilisateurs qui bénéficient du service?

Les utilisateurs titulaires d’une licence Office 365 E5, Microsoft 365 E5, conformité à la réglementation Microsoft 365 E5 et Office 365 Advanced Compliance peuvent bénéficier de la fonctionnalité eDiscovery avancée.

### <a name="how-do-users-benefit-from-the-service"></a>Comment les utilisateurs bénéficient-ils du service?

Les utilisateurs bénéficient d’Advanced eDiscovery lorsque leur contenu est mis en attente dans le cadre d’un litige ou d’une enquête.

### <a name="how-is-the-service-provisioneddeployed"></a>Comment le service est-il configuré/déployé?

Par défaut, les fonctionnalités avancées de découverte électronique sont activées au niveau du client pour tous les utilisateurs au sein du client lorsque les administrateurs affectent des autorisations eDiscovery dans le centre de conformité & Compliance Center.

### <a name="how-can-the-service-be-applied-only-to-users-in-the-tenant-who-are-licensed-for-the-service"></a>Comment le service peut-il être appliqué uniquement aux utilisateurs du client qui sont titulaires d’une licence pour ce service?

Les organisations peuvent gérer Advanced eDiscovery par utilisateur et ajouter des utilisateurs à un cas avancé de découverte électronique, ainsi qu’offrir aux utilisateurs un accès en modification aux emplacements partagés via des autorisations eDiscovery. Pour obtenir des instructions sur l’application des autorisations avancées eDiscovery aux utilisateurs titulaires d’une licence, consultez [la rubrique attribution d’autorisations eDiscovery dans le centre de sécurité & conformité](https://docs.microsoft.com/office365/securitycompliance/assign-ediscovery-permissions).

## <a name="office-365-customer-key"></a>Clé client Office 365

La clé client vous permet de contrôler les clés de chiffrement de votre organisation et de configurer Office 365 afin de les utiliser pour chiffrer vos données au repos dans les centres de données de Microsoft. En d’autres termes, la clé client vous permet d’ajouter une couche de chiffrement qui vous appartient, à l’aide de vos propres clés. Les données de Rest incluent des données à partir d’Exchange Online et de Skype entreprise, qui sont stockées dans des boîtes aux lettres et des fichiers dans SharePoint Online et OneDrive entreprise.

### <a name="which-users-benefit-from-the-service"></a>Quels sont les utilisateurs qui bénéficient du service?

Les utilisateurs titulaires d’une licence Office 365 E5, Microsoft 365 E5, conformité à la réglementation Microsoft 365 E5 et Office 365 Advanced Compliance peuvent bénéficier de la clé client. Pour tirer pleinement parti de la clé client, vous devez également disposer d’un abonnement pour le coffre-fort des clés Azure.

### <a name="how-do-users-benefit-from-the-service"></a>Comment les utilisateurs bénéficient-ils du service?

Les utilisateurs bénéficient de la clé client en faisant en sorte que leurs données soient chiffrées au niveau de la couche d’application à l’aide de clés de chiffrement fournies, contrôlées et gérées par leur propre organisation.

### <a name="how-is-the-service-provisioneddeployed"></a>Comment le service est-il configuré/déployé?

Les clés de chiffrement de clés de client Office 365 peuvent être activées pour toutes les données stockées dans des boîtes aux lettres Exchange Online et Skype entreprise, ainsi que pour les fichiers SharePoint Online et OneDrive entreprise. Pour plus d’informations sur la configuration de la clé de client Office 365 pour chiffrer vos données au repos, consultez [la rubrique contrôle de vos données dans office 365 à l’aide de la clé client](https://docs.microsoft.com/office365/securitycompliance/controlling-your-data-using-customer-key).

### <a name="how-can-the-service-be-applied-only-to-users-in-the-tenant-who-are-licensed-for-the-service"></a>Comment le service peut-il être appliqué uniquement aux utilisateurs du client qui sont titulaires d’une licence pour ce service?

Pour attribuer des clés de chiffrement aux données d’un client Office 365 et/ou Microsoft 365 pour les utilisateurs sous licence, suivez les stratégies de déploiement de clés de chiffrement par clé client:

  - Pour SharePoint Online, les fichiers sur un ou plusieurs sites peuvent être chiffrés à l’aide de la clé client comme décrit ici: [configuration de la clé client pour SharePoint Online et OneDrive entreprise](https://docs.microsoft.com/office365/securitycompliance/controlling-your-data-using-customer-key#office-365-setting-up-customer-key-for-sharepoint-online-and-onedrive-for-business).

  - Pour Exchange Online et Skype entreprise Online, les boîtes aux lettres peuvent être chiffrées à l’aide de la clé client comme décrit ici: [configuration de la clé client pour Exchange Online et Skype entreprise](https://docs.microsoft.com/office365/securitycompliance/controlling-your-data-using-customer-key#office-365-setting-up-customer-key-for-exchange-online-and-skype-for-business)

## <a name="office-365-customer-lockbox"></a>Demandes Customer Lockbox dans Office 365

Le référentiel sécurisé du client fournit une couche supplémentaire de contrôle en offrant aux clients la possibilité d’accorder une autorisation d’accès explicite pour les opérations de service. En démontrant que des procédures sont en place pour autoriser l’accès explicite aux données, le référentiel sécurisé du client peut également aider les organisations à respecter certaines obligations de conformité telles que HIPAA et FEDRAMP.

### <a name="which-users-benefit-from-the-service"></a>Quels sont les utilisateurs qui bénéficient du service?

Les utilisateurs titulaires d’une licence Office 365 E5, Microsoft 365 E5, conformité à la réglementation Microsoft 365 E5 et la conformité avancée d’Office 365 peuvent bénéficier de la zone de sécurité du client.

### <a name="how-do-users-benefit-from-the-service"></a>Comment les utilisateurs bénéficient-ils du service?

Les utilisateurs bénéficient du référentiel sécurisé du client s’assurer que personne de Microsoft ne peut accéder à leur contenu pour effectuer une opération de service sans l’approbation explicite du client. Le référentiel sécurisé du client place le client dans le flux de travail d’approbation pour les demandes d’accès à son contenu. Parfois, des ingénieurs Microsoft sont impliqués lors du processus de prise en charge pour dépanner et résoudre les problèmes signalés par les clients. Dans la plupart des cas, les problèmes sont résolus par des outils de télémétrie et de débogage complets que Microsoft a en place pour ses services. Toutefois, dans certains cas, un ingénieur Microsoft peut accéder au contenu client pour déterminer la cause première et résoudre le problème. Le référentiel sécurisé du client exige que l’ingénieur demande l’accès au client en tant que dernière étape du flux de travail approbation. Les organisations peuvent ainsi approuver ou refuser ces demandes, ce qui leur permet de contrôler directement si un ingénieur Microsoft peut accéder aux données de l’utilisateur final de l’organisation.

### <a name="how-is-the-service-provisioneddeployed"></a>Comment le service est-il configuré/déployé?

Les administrateurs peuvent activer les contrôles de référentiel sécurisé du client dans le centre d’administration Microsoft 365. Pour plus d’informations, consultez la rubrique [Customer Lockbox in Office 365](https://docs.microsoft.com/Office365/Admin/manage/customer-lockbox-requests). Lorsque le référentiel sécurisé est activé, Microsoft est tenu d’obtenir l’approbation d’une organisation avant d’accéder à son contenu.

### <a name="how-can-the-service-be-applied-only-to-users-in-the-tenant-who-are-licensed-for-the-service"></a>Comment le service peut-il être appliqué uniquement aux utilisateurs du client qui sont titulaires d’une licence pour ce service?

Microsoft ne s’engage pas à fournir des demandes d’approbation de contrôle d’accès bte post. Au fil du temps, les vérifications de licence ou les outils ciblés seront ajoutés au référentiel sécurisé du client pour s’assurer que le référentiel sécurisé est accessible aux utilisateurs titulaires d’une licence.

## <a name="privileged-access-management-in-office-365"></a>Gestion des accès privilégiés dans Office 365

La gestion des accès privilégiés fournit un contrôle d’accès granulaire sur les tâches d’administration privilégiée dans Office 365. Une fois que vous avez activé la gestion des accès privilégiés, les utilisateurs doivent demander un accès juste-à-temps via un flux de travail d’approbation hautement étendu et lié au temps afin de réaliser des tâches élevées et privilégiées.

### <a name="which-users-benefit-from-the-service"></a>Quels sont les utilisateurs qui bénéficient du service?

Les utilisateurs titulaires d’une licence Office 365 E5, Microsoft 365 E5, conformité à la réglementation Microsoft 365 E5 et Office 365 Advanced Compliance peuvent tirer parti de PAM.

### <a name="how-do-users-benefit-from-the-service"></a>Comment les utilisateurs bénéficient-ils du service?

L’activation de PAM permet aux organisations de fonctionner avec des privilèges autonomes. Les utilisateurs bénéficient de la couche de défense supplémentaire contre les vulnérabilités résultant d’un accès administratif permanent qui procure un accès non plus fiable à leurs données.

### <a name="how-is-the-service-provisioneddeployed"></a>Comment le service est-il configuré/déployé?

Par défaut, les fonctionnalités de PAM sont activées au niveau du client pour tous les utilisateurs au sein du client. Pour plus d’informations sur la configuration des stratégies de PAM, consultez la rubrique [configuration de la gestion des accès privilégiés dans Office 365](https://docs.microsoft.com/office365/securitycompliance/privileged-access-management-configuration).

### <a name="how-can-the-service-be-applied-only-to-users-in-the-tenant-who-are-licensed-for-the-service"></a>Comment le service peut-il être appliqué uniquement aux utilisateurs du client qui sont titulaires d’une licence pour ce service?

Les clients peuvent gérer le module PAM par utilisateur grâce à des stratégies de groupe et d’accès approbateur, qui peuvent être appliquées aux utilisateurs sous licence. Pour plus d’informations, consultez la rubrique [gestion des accès privilégiés dans Office 365](https://techcommunity.microsoft.com/t5/Security-Privacy-and-Compliance/Privileged-access-management-in-Office-365-is-now-Generally/ba-p/261751).

## <a name="data-loss-prevention-for-exchange-online-sharepoint-online-and-onedrive-for-business"></a>Protection contre la perte de données pour Exchange Online, SharePoint Online et OneDrive entreprise

Avec la protection contre la perte de données (DLP) pour Exchange Online, SharePoint Online et OneDrive entreprise, les organisations peuvent identifier, surveiller et protéger automatiquement les informations sensibles dans les e-mails et les fichiers (y compris les fichiers stockés dans le fichier Microsoft teams référentiels).

### <a name="which-users-benefit-from-the-service"></a>Quels sont les utilisateurs qui bénéficient du service?

Les utilisateurs sous licence d’Office 365 E3, Microsoft 365 E3 et Office 365 Data Loss protection peuvent tirer parti de DLP pour Exchange Online, SharePoint Online et OneDrive entreprise.

### <a name="how-do-users-benefit-from-the-service"></a>Comment les utilisateurs bénéficient-ils du service?

Les utilisateurs bénéficient de DLP pour Exchange Online, SharePoint Online et OneDrive entreprise lorsque leurs courriers électroniques et fichiers sont inspectés pour obtenir des informations sensibles, comme configuré dans la stratégie DLP de l’organisation.

### <a name="how-is-the-service-provisioneddeployed"></a>Comment le service est-il configuré/déployé?

Par défaut, les messages électroniques Exchange Online, les sites SharePoint et les comptes OneDrive sont des *emplacements activés (charges de travail)* pour ces fonctionnalités DLP pour tous les utilisateurs au sein du client. Pour plus d’informations sur l’utilisation des stratégies DLP, consultez la rubrique [vue d’ensemble de la protection contre la perte de données](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies).

### <a name="how-can-the-service-be-applied-only-to-users-in-the-tenant-who-are-licensed-for-the-service"></a>Comment le service peut-il être appliqué uniquement aux utilisateurs du client qui sont titulaires d’une licence pour ce service?

Les administrateurs peuvent personnaliser les emplacements (charges de travail), les utilisateurs et les utilisateurs exclus dans le centre de sécurité & de la sécurité Office 365, sous**emplacements**de **protection contre** > la perte de données.

## <a name="data-loss-prevention-for-teams-chat-and-channel-conversations"></a>Protection contre la perte de données pour les conversations de conversation et de canal teams

Grâce à la protection contre la perte de données (DLP) pour les conversations de conversation et de canal de teams, les organisations peuvent bloquer les messages dans les conversations et les conversations de canal contenant des informations sensibles, telles que des informations financières, des informations d’identification personnelle informations relatives à l’état de santé ou autres informations confidentielles.

### <a name="which-users-benefit-from-the-service"></a>Quels sont les utilisateurs qui bénéficient du service?

Les utilisateurs titulaires d’une licence Office 365 E5, Microsoft 365 E5, conformité à la réglementation Microsoft 365 E5 et Office 365 Advanced Compliance peuvent tirer parti de DLP pour les conversations de conversation et de canal.

### <a name="how-do-users-benefit-from-the-service"></a>Comment les utilisateurs bénéficient-ils du service?

Les expéditeurs bénéficient des informations sensibles dans leurs messages de conversation et de conversation de canal sortants inspectés pour obtenir des informations sensibles, comme configuré dans la stratégie DLP de l’organisation.

### <a name="how-is-the-service-provisioneddeployed"></a>Comment le service est-il configuré/déployé?

Par défaut, la conversation de teams et les conversations de canal sont un *emplacement activé (charge de travail)* pour ces fonctionnalités DLP pour tous les utilisateurs au sein du client. Pour plus d’informations sur l’utilisation des stratégies DLP, consultez la rubrique [vue d’ensemble de la protection contre la perte de données](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies).

### <a name="how-can-the-service-be-applied-only-to-users-in-the-tenant-who-are-licensed-for-the-service"></a>Comment le service peut-il être appliqué uniquement aux utilisateurs du client qui sont titulaires d’une licence pour ce service?

Les administrateurs peuvent personnaliser les emplacements (charges de travail), les utilisateurs et les utilisateurs exclus dans le centre de sécurité & de la sécurité Office 365, sous**emplacements**de **protection contre** > la perte de données.

## <a name="information-barriers"></a>Barrières des informations

Les barrières d’informations sont des stratégies qu’un administrateur peut configurer pour empêcher des personnes ou des groupes de communiquer entre eux. Ceci est utile si, par exemple, un service gère des informations qui ne doivent pas être partagées avec d’autres services, ou si un groupe ne doit pas être en mesure de communiquer avec des contacts externes. Les stratégies de barrière des informations empêchent également les recherches et la découverte. Cela signifie que si vous tentez de communiquer avec une personne avec laquelle vous ne devez pas communiquer, vous ne trouverez pas cet utilisateur dans le sélecteur de personnes.

### <a name="which-users-benefit-from-the-service"></a>Quels sont les utilisateurs qui bénéficient du service?

Les utilisateurs titulaires d’une licence Office 365 E5, Microsoft 365 E5, conformité à la réglementation Microsoft 365 E5 et Office 365 Advanced Compliance peuvent tirer parti des barrières de l’information.

### <a name="how-do-users-benefit-from-the-service"></a>Comment les utilisateurs bénéficient-ils du service?

Les utilisateurs bénéficient des fonctionnalités de conformité avancées des barrières d’information lorsqu’ils ne sont pas autorisés à communiquer avec d’autres personnes. Par exemple :

| Scénario                                                                                                                                                                                                              | Qui a besoin d’une licence? |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------- |
| Deux groupes (groupe 1 et groupe 2) ne peuvent pas communiquer les uns avec les autres (autrement dit, les utilisateurs du groupe 1 ne sont pas autorisés à communiquer avec les utilisateurs du groupe 2, et les utilisateurs du groupe 2 ne sont pas autorisés à communiquer avec les utilisateurs du groupe 1. | Utilisateurs dans les groupes 1 et 2                    |
| Les utilisateurs du groupe 1 ne sont pas autorisés à communiquer avec le reste de l’entreprise.                                                                                                                                       | Utilisateurs du groupe 1 uniquement                                |
| Le reste de la société ne peut pas communiquer avec le groupe 1.                                                                                                                                                 | Tous les utilisateurs à l’exception de ceux du groupe 1                    |
| Les utilisateurs du groupe 1 ne sont pas autorisés à communiquer avec les utilisateurs du groupe 2, mais les utilisateurs du groupe 2 peuvent communiquer avec les utilisateurs du groupe 1.                                                                                              | Utilisateurs du groupe 1 uniquement                                |

### <a name="how-is-the-service-provisioneddeployed"></a>Comment le service est-il configuré/déployé?

Les administrateurs créent et gèrent des stratégies de barrière des informations à l’aide des applets de commande PowerShell dans le centre de sécurité & conformité. Les administrateurs doivent se voir attribuer le rôle administrateur général de Microsoft 365 entreprise, administrateur général Office 365 ou administrateur de conformité pour créer une stratégie de barrière des informations. Par défaut, ces stratégies s’appliquent à tous les utilisateurs du client. Pour plus d’informations sur les barrières d’informations, consultez la rubrique [barrières relatives aux informations dans Microsoft teams](https://docs.microsoft.com/MicrosoftTeams/information-barriers-in-teams).

### <a name="how-can-the-service-be-applied-only-to-users-in-the-tenant-who-are-licensed-for-the-service"></a>Comment le service peut-il être appliqué uniquement aux utilisateurs du client qui sont titulaires d’une licence pour ce service?

Les administrateurs peuvent personnaliser les emplacements (charges de travail), les utilisateurs et les utilisateurs exclus dans le centre de sécurité & conformité d’Office 365. Par exemple, si tous les utilisateurs disposent d’une licence pour Office 365 E3 et qu’aucun ne dispose d’une licence pour Office 365 Advanced Compliance/E5, ils n’ont pas besoin de créer de stratégies de barrière des informations pour l’organisation. Pour plus d’informations, consultez la rubrique [barrières relatives aux informations dans Microsoft teams](https://docs.microsoft.com/MicrosoftTeams/information-barriers-in-teams).

## <a name="office-365-advanced-message-encryption"></a>Chiffrement de messages avancé Office 365

Le chiffrement de messages avancé aide les clients à respecter les obligations de conformité qui nécessitent des contrôles plus souples pour les destinataires externes et leur accès aux messages chiffrés. Avec le chiffrement de messages avancé, les administrateurs peuvent contrôler les messages électroniques sensibles partagés en dehors de l’organisation à l’aide de stratégies automatiques pouvant détecter des types d’informations sensibles (par exemple, des informations d’identification personnelle ou des ID financiers ou d’intégrité) ou ils peuvent utiliser des mots clés pour améliorer la protection en appliquant des modèles de courrier personnalisés et en expirant l’accès à des e-mails chiffrés via un portail Web sécurisé. En outre, les administrateurs peuvent contrôler les messages électroniques chiffrés accessibles en externe via un portail Web sécurisé en révoquant l’accès à tout moment.

### <a name="which-users-benefit-from-the-service"></a>Quels sont les utilisateurs qui bénéficient du service?

Les utilisateurs titulaires d’une licence Office 365 E5, Microsoft 365 E5, conformité à la réglementation Microsoft 365 E5 et Office 365 Advanced Compliance peuvent bénéficier du chiffrement de messages avancé.

### <a name="how-do-users-benefit-from-the-service"></a>Comment les utilisateurs bénéficient-ils du service?

Les expéditeurs de messages bénéficient d’un contrôle supplémentaire sur les messages électroniques sensibles fournis par le chiffrement de messages avancé.

### <a name="how-is-the-service-provisioneddeployed"></a>Comment le service est-il configuré/déployé?

Les administrateurs créent et gèrent des stratégies de chiffrement de messages avancées dans le centre d’administration Exchange sous règles de flux de messagerie. Par défaut, ces règles s’appliquent à tous les utilisateurs sur le client. Pour plus d’informations sur la configuration des nouvelles fonctionnalités de chiffrement des messages, consultez la rubrique [set up New Office 365 message Encryption Capabilities](https://docs.microsoft.com/office365/securitycompliance/set-up-new-message-encryption-capabilities).

### <a name="how-can-the-service-be-applied-only-to-users-in-the-tenant-who-are-licensed-for-the-service"></a>Comment le service peut-il être appliqué uniquement aux utilisateurs du client qui sont titulaires d’une licence pour ce service?

Les administrateurs doivent appliquer des règles de flux de messagerie pour le chiffrement de messages avancé uniquement aux utilisateurs titulaires d’une licence. Pour plus d’informations sur la définition des règles de flux de messagerie, voir [définir des règles de flux de messagerie pour chiffrer les messages électroniques dans Office 365](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email).