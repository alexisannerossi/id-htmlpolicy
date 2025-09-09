---
title: RFC Policy for HTML and CSS formats
docname: draft-rossi-htmlpolicy-00
venue:
  group: RSWG
  type: Editorial Stream Working Group
  mail: rswg@rfc-editor.org
  arch: https://mailarchive.ietf.org/arch/browse/rswg/
  github: "alexisannerossi/id-svgsinrfcs"
  latest: "https://github.com/alexisannerossi/id-htmlpolicy/blob/main/id-htmlpolicy.md"
stand_alone: true
v: 3
obsoletes: 7992, 7993
ipr: trust200902
kw: Internet-Draft
cat: info
submissionType: editorial
keyword:
 - HTML
author:
  -
    ins: P. Hoffman
    name: Paul Hoffman
    organization: ICANN
    email: paul.hoffman@icann.org
  -
    ins: A. Rossi
    name: Alexis Rossi
    organization: RFC Series Consulting Editor
    email: rsce@rfc-editor.org

normative:


informative:
  RFC7992:
  RFC7993:
  WAI:
    author:
      org: W3C
    title: W3C Accessibility Standards Overview
    target: https://www.w3.org/WAI/standards-guidelines/

--- abstract

This document sets policy for the HTML publication format and supporting CSS files for RFCs. It contains policy requirements, some of which are taken from {{RFC7992}} and {{RFC7993}}, and removes any specific implementation or tooling requirements imposed by {{RFC7992}} or {{RFC7993}}.

--- middle

# Introduction

This document sets policy for the HTML publication format and supporting CSS files for RFCs. It contains policy requirements, some of which are taken from {{RFC7992}} and {{RFC7993}}, and removes any specific implementation or tooling requirements imposed by {{RFC7992}} or {{RFC7993}}.

The RFC Publication Center (RPC) is responsible for the HTML publication format and CSS file tooling and implementation decisions. They may want to use the contents of {{RFC7992}} and {{RFC7993}} as a starting point for documenting those decisions, but they are not bound by {{RFC7992}} or {{RFC7993} and they may change elements of the implementation as needed to support the RFC authoring community as long as those changes are aligned with the policy requirements in this document.

# Policy Requirements

HTML publication format and CSS file tooling and implementation decisions are made or overseen by the RPC, and must adhere to the following policy requirements.

* The HTML and CSS must not alter or change the display of an RFC in any way that would affect a reader's ability to identify and understand the original semantic content.
* The HTML must render correctly on a list of common devices and browser versions that the RFC Editor will keep up to date outside of this document.
* The RPC must consider both the probable longevity of wide support and the security implications for their implementation decisions.
* The HTML must display adequately in at least one text-based browser. 
* The HTML document must be self-contained, without requiring external files for images, CSS, JavaScript, or the like.
* HTML tags should rarely have attributes whose only purpose is to affect the rendered styling, and those should only be used if it is not possible to specify that styling in CSS.
* JavaScript may be supported, but care should be taken to prevent any JavaScript that might alter the semantic content of the RFC.
* All sections, subsections, figures, and paragraphs should have stable numbered link anchors that can be used to facilitate navigation to and sharing of specific content within the document. Both user-defined and auto-generated anchors must be supported and linkable. 
* The HTML should be as accessible as possible to people with visual disabilities, including those who have color blindness, those who need to scale or change fonts, and those who use screen reading software. This may include allowing easy local override of the default CSS formatting. This policy does not preclude the use of features that are not accessible, as long as those inaccessible features do not take the place of or hamper the usability of accessible features. The accessibility of the RFC's semantic content should be prioritized. The RPC will refer to the W3C Accessibility Guidelines {{WAI}} when making decisions regarding accessibility. 
* The HTML and CSS produced for Internet-Drafts may differ from that produced by the RPC for RFC publication.
* The HTML should be constructed in a way to allow search engines to discover and extract appropriate content, or to improve search engine optimization (SEO), as long as it avoids changing any semantic content of the RFC.
* HTML and CSS implementation may change over time. Changes are not required to remain backwards-compatible, although maintaining compatibility where possible is encouraged.

The RPC is authorized to make decisions about the HTML publication format and CSS for both technical and editorial reasons in order to ensure that published RFCs meet the above policy and to provide consistency across the RFC series.
The RPC must document their HTML publication format and CSS decisions in a public place, and all changes to tooling or implementation decisions must be widely communicated to the RFC author community using mailing lists or other means.

# Implementation Guidance

The RPC is expected to solicit community input before making decisions and to publicly explain their reasoning.

Documentation produced by the RPC should describe what technical and editorial constraints apply to the HTML publication format and CSS files.

Where possible, implementation decisions should focus on specifying what is disallowed, rather than attempting to specify exactly what is allowed.

The RPC should periodically review and revise their practices.

# Security Considerations

This document has no security considerations.


# IANA Considerations

This document has no IANA actions.

# Acknowledgements

Thank you to Joe Hildebrand, Paul E. Hoffman, and Heather Flanagan for their extensive work in {{RFC7992}} and {{RFC7993}}. These documents are foundational to the publication of the series, and underlie many of the policies in this document.

--- back
