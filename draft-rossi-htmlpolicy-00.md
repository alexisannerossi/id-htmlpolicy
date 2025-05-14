---
title: RFC Policy for the HTML publication format
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
obsoletes: 7992
ipr: trust200902
kw: Internet-Draft
cat: info
submissionType: editorial
keyword:
 - HTML
author:
  -
    ins: A. Rossi
    name: Alexis Rossi
    organization: RFC Series Consulting Editor
    email: rsce@rfc-editor.org


normative:


informative:
  RFC7992:
  WAI:
    author:
      org: W3C
    title: W3C Accessibility Standards Overview
    target: https://www.w3.org/WAI/standards-guidelines/

--- abstract

This document sets policy for the HTML publication format for RFCs. It contains policy requirements, some of which are taken from {{RFC7992}}, and removes any specific implementation or tooling requirements imposed by {{RFC7992}}.

--- middle

# Introduction

This document sets policy for the HTML publication format for RFCs. It contains policy requirements, some of which are taken from {{RFC7992}}, and removes any specific implementation or tooling requirements imposed by {{RFC7992}}.

The RFC Publication Center (RPC) is responsible for HTML publication format tooling and implementation decisions. They may want to use the content of {{RFC7992}} as a starting point for documenting those decisions, but they are not bound by {{RFC7992}} and they may change elements of the implementation as needed to support the RFC authoring community as long as those changes are aligned with the policy requirements in this document.

# Policy Requirements

HTML publication format tooling and implementation decisions are made or overseen by the RPC, and must adhere to the policy requirements in this document.

* The visual layout of the document will be defined through a cascading style sheet (CSS)

The RPC is authorized to make decisions about the HTML publication format for both technical and editorial reasons
in order to ensure that published RFCs meet the above policy and to provide consistency across the RFC series.
The RPC must document their HTML publication format decisions, and all changes to tooling or implementation decisions must be widely communicated to the RFC author community using mailing lists or other means.

# Implementation Guidance

The RPC is expected to solicit community input before making decisions and to publicly explain their reasoning.

Documentation produced by the RPC should describe what technical and editorial constraints apply to the HTML publication format.

Where possible, implementation decisions should focus on specifying what is disallowed, rather than attempting to specify exactly what is allowed.

The RPC should periodically review and revise their practices.

# Security Considerations

This document has no security considerations.


# IANA Considerations

This document has no IANA actions.


--- back
