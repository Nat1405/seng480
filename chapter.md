# Zulip <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/33/Zulip_logo.svg/1280px-Zulip_logo.svg.png" width="20" height="20"> 

## Table Of Contents

 1. Purpose
 2. About Zulip
 3. Stakeholders
 4. Business Goals
 5. Architecturally Significant Requirements (ASR)
 6. Utility Tree
 7. Quality Attribute Scenarios (QAS)
 8. Module View
    * Primary Presentation
    * Element Catalog
      + Elements and Properties
      + Relations and Properties
      + Element Behaviour
    * Context Diagram
    * Rationale
 9. Component and Connector View
    * Primary Presentation
    * Element Catalog
      + Elements and Properties
      + Relations and Properties
      + Element Behaviour
    * Context Diagram
    * Variability Guide
    * Rationale
 10. Code Quality and Technical Debt
 11. Conclusion
 
## Team 

## Purpose

## About Zulip

## Privacy, Security, and Ethics

#### 1 Introduction
#### 2 Potential Privacy and Security Concerns

This section assesses how Zulip currently complies with the [ACM Code of Ethics and Professional Conduct](https://www.acm.org/code-of-ethics) with regards to privacy and security. These issues are particularly relevant as this chat application is intended for company use and will be transferring potentially confidential information. Zulip supports compliance with GDPR and HIPAA, which are data privacy standards for the European Union and the United States, respectively.

Zulip provides a fairly concise and transparent account of its data usage procedures on its [website]( https://zulipchat.com/privacy/). However, the policy fails to adequately describe the policies for data retention and disposal. Whereas the Code of Ethics section 1.6 states that this information "should be clearly defined, enforced, and communicated to data subjects", the privacy policy does not specify how long data is retained. In fact, Zulip states that even after deleting information from Zulip's services, "we may not immediately delete residual copies from our active servers and may not remove information from our backup systems."

In addition, although you may deactivate your account as a user, it is unclear how to have your personal information deleted. The privacy policy only mentions that Zulip will provide ways to delete your information in the case that the information is wrong. Another issue is that your messages and shared files will remain visible even after deactivating your account. The only workaround appears to be manually removing this information before deactivating your account.

Because Zulip allows users to deploy their own server, it is important that the security features of Zulip are simple to use and well-documented. Zulip provides a [short overview](https://zulip.readthedocs.io/en/stable/production/security-model.html) of its security features. To supplement this, there is a Zulip community server providing product support, as well as a Google group for users to report security bugs and receive security updates. In accordance with the Code of Ethics, the Zulip development team seems responsive to security bugs, issuing 3 dedicated security patches out of the last 13 updates. As with other chat apps, a Zulip server may be vulnerable to its users unintentionally exposing data through the misuse of 3rd party integrations, as well as through administrators failing to deactivate old accounts, such as those for ex-employees.

#### 3 Ethical Dilemmas

This section will attempt to analyze potential ethical dilemmas that Zulip will face as an open source project. Since Zulip is a chat application the vast majority of potential ethical problems stem from privacy and confidentiality issues, and that is where we have focused our analysis. 

One potential Ethical Dilemma that Zulip faces is the potential influence of paying users, corporate or otherwise, to influence the project. Unlike many other open source projects Zulip offers [multiple payment plans for potential users](https://zulipchat.com/plans/) including a standard paid version and, more importantly, an Enterprise payment plan which offers the benefit "Input into the Zulip roadmap." It is possible for this option to influence influence the direction of the project in a way that disproportionately favours enterprises that heavily fund Zulip exists, and Zulip will need to understand when this is happening, and decide whether the funding is valuable enough to outweigh the potential downsides. 

Because Zulip stores the private messages and data of users, provided they are not hosting their own server, there is the potential that incriminating messages will be sent using the platform. This has the potential to lead to a situation where Zulip must decide whether or not the chat logs and data will be released to the authorities or if the privacy of the users will be prioritized. This dilemma falls broadly under section 1.6 and 1.7 of the [ACM Code of Ethics and Professional Conduct](https://www.acm.org/code-of-ethics), Respect Privacy and Honor Confidentiality respectively. If Zulip is ever faced with this choice they will need to evaluate their stance as a company and set a precedent for all future decisions of this type. 

A final issue that Zulip may be faced with in the future is one of free speech. As has been seen on multiple social media platforms in recent years, such as [Facebook](https://globalnews.ca/news/5141557/facebook-bans-extremism-hate-policy/) and [Reddit](https://www.theverge.com/2019/3/15/18267645/reddit-watchpeopledie-ban-new-zealand-mosque-massacre-christchurch),the possibility of an individual or group starting a potentially offensive or dangerous group on Zulip is entirely possible. This issue is further clouded by Zulip's allowance of users to host the application off of their own servers. In the future Zulip may have to make case by case decisions on whether or not to allow groups to exist on their application. 

#### 4 Summary
#### 5 Sources (issue tracker discussion, wiki/web pages, commit comments, media reports).


## Stakeholders

| Role | Concerns | Instances |
|-----|----------|-----------|
| Acquirers |	Oversee the procurement of the system or product | |
| Assessors |	Oversee the system’s conformance to standards and legal regulation | |
| Communicators |	Explain the system to other stakeholders via its documentation and training materials | |
| Developers |	Construct and deploy the system from specifications (or lead the teams that do this) | |
| Maintainers |	Manage the evolution of the system once it is operational | |
| Production  Engineers |	Design, deploy, and manage the hardware and software environments in which the system will be built, tested,  and run | |
| Suppliers |	Build and/or supply the hardware, software, or infrastructure on which the system will run | |
| Support  Staff |	Provide support to users for the product or system when it is running | |
| System Administrators	| Run the system once it has been deployed | |
| Testers |	Test the system to ensure that it is suitable for use | |
| Users |	Define the system’s functionality and ultimately make use of it | |
