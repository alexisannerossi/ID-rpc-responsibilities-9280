---
title: "RPC Roles and Responsibilities"
abbrev: "RPCResponsibilities"
category: info

docname: draft-rossi-rpcresponsibilities-latest
submissiontype: IETF  # also: "independent", "editorial", "IAB", or "IRTF"
number:
date:
consensus: true
v: 3
# area: AREA
# workgroup: WG Working Group
keyword:
 - RFC Publication Formats
updates: 7990, 7991, 7992, 7993, 7994, 7995, 7996, 7997, 9280

venue:
#  group: RSWG
#  type: Working Group
#  mail: rswg@rfc-editor.org
#  arch: https://datatracker.ietf.org/edwg/rswg/
  github: "ID-rpc-responsibilities-9280"
  latest: "https://alexisannerossi.github.io/ID-rpc-responsibilities-9280/draft-rossi-rpcresponsibilities.html"

author:
 -
    fullname: "Alexis Rossi"
    organization: RFC Series Consulting Editor
    email: "rsce@rfc-editor.org"

--- abstract

This document updates RFC 9280 to specify that the RPC is responsible for operational decisions needed to implement RFC Series policies as they pertain to the document publication process code and tools, and provides a pathway for resolution of disagreements with those operational decisions. This document also updates RFC9280 to acknowledge that RFC Consumers, a distinct but partially overlapping group with IETF participants, must be specifically considered in the process of writing and implementing RFC Series policies, and makes the RPC responsible for representing their interests. Additionally, this document updates language in RFC7990, RFC7991, RFC7992, RFC7993, RFC7994, RFC7995, RFC7996, and RFC7997 to transfer responsibilities previously held by the RFC Editor or RFC Series Editor to the RPC.


--- middle


# Introduction

RFC Editor Model (Version 3) {{!RFC9280}} created a new structure for the RFC Editor function, establishing the RFC Series Working Group (RSWG) and the RFC Series Approval Board (RSAB) and giving new responsibilities to the RFC Production Center (RPC). Broadly speaking, it says that RSWG writes policies for the editorial stream, RSAB approves those policies, and the RPC implements those policies. 

However RFC 9280 does not specify which group is responsible for defining or building the specific code and tools that implement the policies agreed upon in this process. 

This document updates RFC 9280 to specify that the RPC is responsible for the development of tools and processes used to implement editorial stream policies, in the absence of an RFC with specific requirements. The RPC may designate a team of volunteers and/or employees who implement these operational decisions. The RPC is expected to solicit input from experts and community members when making implementation decisions. The RPC is required to document implementation decisions in a publicly available place, preferably with rationale.

While RFC 9280 provides a pathway for resolution of conflict between the RPC and the author(s) of a specific document (RFC 9280 section 4.4), no appeal pathway is given for resolution of issues that may occur when a community member believes an RPC implementation decision that applies to the entire publication process (not just one document) conflicts with an RFC Series policy. This document defines that both types of appeals will follow the same path (appeal to RSAB).

This document formally defines the term “Consumers of RFCs”, defines the policy to be applied by the RFC publication streams (currently IETF, IRTF, IAB, Independent Stream and Editorial Stream) and the RFC Editor in respect of consumers of RFCs, and defines the role of the RPC in representing consumers of RFCs in the Editorial Stream process defined in RFC 9280.

Finally, the set of RFCs that define our current publication formats (RFC 7990, RFC 7991, RFC 7992, RFC 7993, RFC 7994, RFC 7995, RFC 7996, and RFC 7997) frequently give responsibility to “the RFC Editor” or “the RFC Series Editor” for implementation decisions. The role of “RFC Editor” that existed when those documents were published was divided into different roles in RFC 9280, so it is unclear who the responsibilities fall to after this split. This document defines that all responsibilities previously held by the RFC Editor or RFC Series Editor in these documents are now held by the RPC. If the RPC has questions about how to interpret policy in these documents, they will refer to RSAB for guidance per the process described in RFC 9280 (RFC 9280 section 4.4).


# Updates to 7990-7997

All instances of “RFC Editor” or “RFC Series Editor” in {{!RFC7990}}, {{!RFC7991}}, {{!RFC7992}}, {{!RFC7993}}, {{!RFC7994}}, {{!RFC7995}}, {{!RFC7996}}, and {{!RFC7997}} are replaced by “RFC Production Center (RPC)”. 


#Updates to 9280

(specific updates TBD)


# RPC Implementation Responsibilities

## Tooling and code used for publication of RFCs

The second responsibility defined in the RFC 9280 Model Overview (RFC 9280 section 2) says “Policy implementation through publication of RFCs in all of the streams that form the RFC Series. This is primarily the responsibility of the RFC Production Center (RPC) as contractually overseen by the IETF Administration Limited Liability Company (IETF LLC).” 

The same section also states, “The RPC implements the policies defined by the Editorial Stream in its day-to-day editing and publication of RFCs from all of the streams.” (9280 section 2)

RFC 9280 does not define any other group that is responsible for implementing policies.

Throughout RFC 9280 the RSWG is consistently assigned responsibility for writing policies (not deciding on implementations). The RPC is consistently assigned responsibility for implementing policy decisions, but examples given generally describe decisions made at the single document level. The document does not cover any specific responsibilities for designing and building the tools and code used to publish documents. 

RFC 9280 mentions tool developers twice. It encourages “developers of tools used to author or edit RFCs and Internet-Drafts” to participate in the RSWG (RFC 9280 3.1.1.2), and it says that  “RSAB members should consult with their constituent stakeholders (e.g., authors, editors, tool developers, and consumers of RFCs) on an ongoing basis” (RFC 9280 3.2.1).

RFC 9280 mentions a specific implementation once when discussing the working practices of the RPC. Elided for brevity, it says “In the absence of a high-level policy documented in an RFC or in the interest of specifying the detail of its implementation of such policies, the RPC can document … Guidelines regarding the final structure and layout of published documents. In the context of the XML vocabulary [RFC7991], such guidelines could include clarifications regarding the preferred XML elements and attributes used to capture the semantic content of RFCs.” (9280 section 4.2) RFC 7991 is the only editorial implementation-related RFC mentioned in 9280.

This document updates RFC 9280 to specify that the RPC is responsible for the development of tools and processes used to implement editorial stream policies, in the absence of an RFC with specific requirements. The RPC may designate a team of volunteers and/or employees who implement these operational decisions. The RPC is expected to solicit input from experts and community members when making implementation decisions. The RPC is required to document implementation decisions in a publicly available place, preferably with rationale.

If the  RPC has questions about how to interpret policy in Editorial stream documents, they should ask RSAB for guidance in interpreting that policy per the process described in RFC 9280 (RFC 9280 section 4.4).

## Conflict resolution for implementation decisions

RFC 9280 provides a pathway for resolution of conflicts between the RPC and the author(s) of a specific document (9280 section 4.4). No appeal pathway is given for resolution of issues that may occur when a conflict arises with an implementation decision that applies to the entire editorial process (not just one document).

If the RPC is responsible for interpreting policy decisions at both the document and editorial process tooling level, conflicts on either level will involve interpretation of written policy (or the acknowledgement that policy does not exist to cover a given situation). In any case, the conflict resolution will use the same path of appeal to the RSAB.


# RFC Consumers

## Origin of the term “consumers of RFCs”

The IETF Mission Statement [RFC 3935] is clear that the documents it produces are intended to be consumed by anyone who wishes to implement an IETF protocol or operational recommendation: “to produce high quality, relevant technical and engineering documents that influence the way people design, use, and manage the Internet in such a way as to make the Internet work better.”

RFC 9280 introduces the term “consumers of RFCs”, referring to them as “constituent stakeholders” who should be considered by RSAB when approving Editorial Stream policy documents (RFC 9280 section 3.2.1).

## Formal definition of the term “consumers of RFCs”

“Consumers of RFCs” is defined to mean those people who read RFCs to understand, implement, critique, and research the protocols, operational practices and other content, as found in RFCs. 

## Policy in respect of consumers of RFCs

The policy to be followed by the RFC publication streams and RFC Editor in respect of consumers of RFCs is as follows:

Consumers of RFCs MUST be considered as a separate constituent stakeholder from IETF/IRTF participants. While IETF/IRTF participants and others involved in the development and production of RFCs may be consumers of RFCs, the two are distinct, overlapping sets.

The RFC Editor website (www.rfc-editor.org) MUST be primarily focused on consumers of RFCs.

Consumers of RFCs MUST NOT be required or expected to become IETF/IRTF participants, but it MAY be recommended or suggested that they do so.

## Representation of consumers of RFCs

Responsibility for representing the interests of consumers of RFCs in the Editorial Stream process as defined in RFC 9280, is assigned to the RPC . The RPC SHOULD represent consumers of RFCs to the best of their ability given the information and tools available to them, both within RSWG and as ex-officio members of RSAB. The RPC MAY solicit information from other individuals, groups or experts, or directly from consumers of RFCs, including by tracking traffic or interactions on www.rfc-editor.org within the constraints of the privacy statement available on www.rfc-editor.org.


# Security Considerations

This document has no security considerations.


# IANA Considerations

This document has no IANA actions.


--- back

# Acknowledgments
{:numbered="false"}

