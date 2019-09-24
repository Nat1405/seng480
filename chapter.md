# Zulip <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/33/Zulip_logo.svg/1280px-Zulip_logo.svg.png" width="20" height="20"> 

## Table Of Contents

 1. Purpose
 2. About Zulip
 3. [Stakeholders](#Stakeholders)
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

## Stakeholders

Zulip is an open-source project, and can be used by anyone, however several stakeholders have a significant influence over the development of the project. Kandra Labs Inc. provides a commercial hosted solution (Zulip Cloud) for Zulip, and is run by Tim Abbott, which gives the company a significant stake in Zulip's development. Open-source contributors to Zulip also use the product regularly, giving them a stake in the project.

Stakeholders for the Zulip project have been assigned to relevant categories from Rozanski and Woods' work [[1]](#r1) below:

* **Assessors:** Kandra Labs, Inc. acts as a GDPR-compliant data subprocessor for Zulip cloud services [[2]](#r2). As such, they must ensure that Zulip has all the required features to comply with GDPR. 

* **Communicators:** Documentation for Zulip (published on [zulip.readthedocs.io](https://zulip.readthedocs.io/en/latest/)) is maintained alongside the codebase. The open-source community is responsible for contributing changes to the online documentation as pull requests.

  Tim Abbott and Kandra Labs also maintain a blog for Zulip ([blog.zulip.org](http://blog.zulip.org)) and a [Twitter page](https://twitter.com/zulip?lang=en).

* **Developers:** Zulip was initially developed by the members of Zulip, Inc., a small startup led by [Tim Abbott](https://github.com/timabbott) which was acquired by Dropbox in 2014 [[3]](#r3). After the project was made open-source by Dropbox in 2015, Tim Abbott continued development work with the help of the open-source community.

* **Maintainers:** [Tim Abbott](https://github.com/timabbott) is currently Zulip's most active maintainer. Other members of the core team include [Anders Kaseorg](https://github.com/andersk) and [Rishi Gupta](https://github.com/rishig). Zulip is also maintained by several distributed developers from open-source development programs, most notably [Google Summer of Code](https://summerofcode.withgoogle.com/) and [Google Code-In](https://codein.withgoogle.com/archive/) [[3]](#r3).

* **Production Engineers:** Kandra Labs provisions the infrastructure for Zulip Cloud [[4]](#r4), while members of the open-source community may also deploy on-premise versions of Zulip.

* **Suppliers:** The Zulip project is funded by an SBIR grant from the US National Science Foundation. 

* **Support Staff:** Kandra Labs provides support for Zulip Cloud. For the open-source project, support is provided by Tim Abbott and other members of the open-source community on the [Zulip community server](http://chat.zulip.org). 

* **System Administrators:** Production instances for Zulip Cloud are maintained by Kandra labs. 

* **Testers:** Testing on the Zulip project is done for every pull request. Manual testing of new features is done by PR reviewers (Tim Abbott or another member of the Zulip core team), and regression testing is handled by a suite of automated front-end and back-end tests.

* **Users:** Zulip is used by several corporate and open-source development teams including Akamai, Wikimedia and MariaDB. It is also used by Zulip's own development team to power the [Zulip community server](http://chat.zulip.org). 

## References

1. <a name="r1"></a>Software Systems Architecture, Rozanski and Woods: https://www.viewpoints-and-perspectives.info/home/stakeholders/
2. <a name="r2"></a>Zulip Help, GDPR Compliance: https://zulipchat.com/help/gdpr-compliance
3. <a name="r3"></a>Zulip History: https://zulipchat.com/history/
4. <a name="r4"></a>Zulip Team: https://zulipchat.com/team/