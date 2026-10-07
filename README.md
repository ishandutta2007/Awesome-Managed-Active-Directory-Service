# Awesome-Managed-Active-Directory-Service

## Top Managed Active Directory Service Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on Managed Directory Services, Identity Platforms & Self-Hosted AD Alternatives*  

**Last updated: October 2026**



This repository tracks notable **commercial managed Active Directory platforms** and **open-source projects** that provide directory services, identity management, and AD-compatible authentication — from fully managed cloud directories to self-hosted AD implementations and sovereign IAM alternatives.



**Examples** include AWS Directory Service, Microsoft Entra ID, JumpCloud, Okta Universal Directory, OneLogin, Ping Identity, Google Workspace Directory, ManageEngine ADManager Plus, Frontegg, and Auth0 (the category leaders).



**Open-source emphasis**: Managed Active Directory is anchored by **Samba** as the most feature-rich open-source AD implementation for Linux/UNIX systems, with **Univention Nubus** delivering a sovereign, open-standards IAM alternative for public sector and regulated industries . **FreeIPA** provides Linux-native identity management with AD trust capabilities, while **389 Directory Server**, **OpenLDAP**, and **ApacheDS** deliver LDAP directory foundations . **midPoint** brings comprehensive identity governance and administration, and **LSC-Project** enables directory synchronization . This section is heavily expanded.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[Microsoft Entra ID](https://www.microsoft.com/en-us/security/business/identity-access/microsoft-entra-id)**  

  **The cloud successor to Azure Active Directory** — workforce identity with SSO, conditional access, MFA, and 10,000+ SaaS app integrations . **Free tier with Microsoft 365**; Premium P1/P2 for advanced features . **Best for Microsoft-centric organizations** .



- **[AWS Directory Service](https://aws.amazon.com/directoryservice/)**  

  **AWS's managed directory services** — Microsoft AD, AD Connector, and Simple AD options . **Integrates with AWS workloads and on-premises AD** . **Best for AWS-native directory workloads** .



- **[JumpCloud](https://jumpcloud.com/)**  

  **The cloud directory platform** — unified directory, SSO, device management, and LDAP . **Free for up to 10 users** . **Best for SMBs wanting cloud directory without AD** .



- **[Okta Universal Directory](https://www.okta.com/products/universal-directory/)**  

  **The market-leading independent directory** — multi-tenant user store with profile mastering and app integration . **Best for enterprise identity** .



- **[OneLogin](https://www.onelogin.com/)**  

  **Workforce identity** — directory, SSO, and MFA . **Best for mid-market enterprises** .



- **[Ping Identity](https://www.pingidentity.com/)**  

  **Enterprise identity platform** — SSO, MFA, and identity governance . **Best for large enterprises** .



- **[Google Workspace Directory](https://workspace.google.com/)**  

  **Google's cloud directory** — user management with SSO and Google ecosystem integration . **Best for Google Workspace users** .



- **[ManageEngine ADManager Plus](https://www.manageengine.com/)**  

  **AD management and reporting** — bulk user provisioning, delegation, and compliance reporting . **Best for Windows AD administration** .



- **[Frontegg](https://frontegg.com/)**  

  **Customer identity platform** — multi-tenant SSO, RBAC, and user management for B2B SaaS . **Best for product-led SaaS** .



- **[Auth0](https://auth0.com/)**  

  **Identity platform for developers** — SSO, MFA, and user management with extensibility . **Best for developer-friendly identity** .



## Open-Source GitHub Projects



### Active Directory Implementations



- **[Samba](https://github.com/samba-team/samba)**  

  **The most feature-rich open-source implementation of SMB and Active Directory protocols**, GPL-3.0 licensed . **Functions as an Active Directory Domain Controller or member server** for Linux/UNIX systems . **Provides secure, stable file and print services using SMB and AD protocols including LDAP and Kerberos** . **Samba 4.24.0 is the latest stable release** (March 2026) . **Trade-offs**: Sysvol replication uses an alternative to DFS-R, and trust relationships are experimental with SID filtering limitations . **Best for open-source AD domain controllers** .



- **[Univention Nubus](https://www.univention.com/solutions/alternative-to-microsoft-active-directory/)**  

  **Sovereign Identity & Access Management alternative to Microsoft Entra ID**, open-source . **Based on open standards including OpenID Connect, SAML, and LDAP** — enabling flexible integration into cloud, on-premises, or hybrid environments . **Provides SSO, MFA, and self-service with full data sovereignty** — can operate entirely within sovereign cloud environments or your own data centers . **Containerized with Kubernetes for scalability, or deployable as a virtual machine** with Active Directory integration for seamless embedding into existing structures . **Trusted by public sector institutions including Schleswig-Holstein and school authorities in Fulda and Kassel** . **Best for organizations seeking digital sovereignty without vendor lock-in** .



### Linux-Native Identity Management



- **[FreeIPA](https://github.com/freeipa/freeipa)**  

  **Identity management for Linux/Unix environments**, GPL-3.0 licensed . **Built on 389 Directory Server with MIT Kerberos and Samba components for Windows interoperability** . **Provides LDAP, Kerberos, DNS, certificate management, HBAC, SELinux integration, netgroups, and sudo integration** — Linux-oriented features not available in AD domains . **Important distinction**: FreeIPA is **not an AD-compatible server** — Windows machines cannot join it directly; instead, it establishes **trust relationships** with AD forests . **Best for Linux-centric identity with AD trust** .



### LDAP Directory Servers



- **[389 Directory Server](https://github.com/389ds/389-ds-base)**  

  **Enterprise-class LDAP server from Red Hat**, GPL-3.0 licensed . **Free version of Red Hat Directory Server** with LDAPv3 support and multi-master replication . **Supports synchronization with Active Directory** and can manage thousands of nodes with thousands of operations per second . **The information store for FreeIPA** and the foundation for its Global Catalog implementation . **Best for enterprise LDAP with AD synchronization** .



- **[OpenLDAP](https://github.com/openldap/openldap)**  

  **The standard open-source LDAP directory**, OpenLDAP Public License . **Widely regarded as the reference implementation** — historically based on the original University of Michigan code base . **C-based for performance** — runs faster than Java implementations on modest hardware . **Complex to configure** compared to alternatives, but supports multi-master replication and RFC 4533 . **Best for large-scale LDAP deployments with operational expertise** .



- **[ApacheDS](https://github.com/apache/directory-server)**  

  **Java-based LDAP server from Apache**, Apache-2.0 licensed . **LDAPv3 certified with Kerberos 5, multi-master replication, password policies, and X500 authorization** . **Managed via Apache Directory Studio** — an Eclipse-based LDAP browser and directory client . **Cross-platform** — runs on any JVM-compatible system . **Best for Java-centric environments and cross-platform LDAP** .



### Identity Governance & Administration



- **[midPoint](https://github.com/Evolveum/midpoint)**  

  **The leading open-source identity governance and administration platform**, Apache-2.0/EUPL licensed . **Recognized by Gartner as a comprehensive IGA suite** — combining identity management with governance . **Handles up to tens of millions of identities** with advanced synchronization and smart correlation using fuzzy search . **Features simulations, role mining with AI algorithms, license management, user self-service, and compliance support for ISO 27001, NIS2, DORA, and GDPR** . **Used by higher education, financial services, government, telco, healthcare, and manufacturing** . **Best for enterprise identity governance** .



- **[LSC-Project (LDAP Synchronization Connector)](https://github.com/lsc-project/lsc)**  

  **Open-source identity synchronization between LDAP directories and other systems**, Apache-2.0 licensed . **Synchronizes identities between LDAP and Active Directory, MySQL, PostgreSQL, and group management systems** . **Supports LDAP, LDAPS, Kerberos, and SSL/TLS protocols** with incremental synchronization and error handling . **Configuration via ini files with runtime modification and plugin extensibility** . **Best for directory synchronization and migration** .



### Additional Strong Open-Source Options



- **OpenDJ** — ForgeRock's Java-based LDAP directory (CDDL 1.0)  .

- **OpenICF.Net** — Identity connector framework for .NET integrating with Active Directory, Exchange, and PowerShell  .

- **jis-iam-bridge** — Bridges legacy IAM (AD, LDAP, SAML, OAuth) to cryptographic identity without rip-and-replace migration  .

- **Samba AD in Docker** — Containerized Samba4 AD Domain Controller for testing and development  .



**Frameworks for building custom managed Active Directory solutions**: Combine **Samba** for open-source AD domain controller functionality with LDAP and Kerberos . Use **Univention Nubus** for sovereign IAM with OpenID Connect, SAML, and LDAP that can replace or complement Entra ID . Deploy **FreeIPA** for Linux-native identity management with AD trust relationships . Choose **389 Directory Server** or **OpenLDAP** for LDAP foundations with AD synchronization . Integrate **midPoint** for comprehensive identity governance and administration . Use **LSC-Project** for directory synchronization between LDAP and AD . Note that true managed AD with global infrastructure, automatic scaling, and vendor-supported SLAs (Entra ID, AWS Directory Service, Okta) remains primarily commercial territory; open-source stacks provide strong AD implementations, LDAP servers, and IGA platforms that require integration for complete managed directory services.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Active Directory and identity management platforms handle sensitive authentication data and access controls. Self-hosted solutions require proper security hardening, access controls, and compliance with data privacy regulations.

- **Samba AD is production-stable** but has limitations: Sysvol replication uses an alternative to DFS-R, trust relationships are experimental with SID filtering limitations, and network browsing is not supported .

- **FreeIPA is not AD-compatible** — Windows machines cannot join it directly. Trust relationships with AD are the supported integration path .

- **License considerations**: Samba uses GPL-3.0, 389 Directory Server uses GPL-3.0, OpenLDAP uses OpenLDAP Public License, ApacheDS uses Apache-2.0, midPoint uses Apache-2.0/EUPL, and Nubus is open-source .

- The open-source ecosystem provides strong AD implementations, LDAP servers, and IGA platforms, but **global infrastructure, managed SLAs, and vendor-supported enterprise features** remain primarily commercial offerings.



---



**Made for system administrators, identity architects, and organizations seeking Active Directory sovereignty.**

Let's make managed Active Directory services more open, transparent, and sovereign.
