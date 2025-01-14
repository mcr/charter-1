Introduction
============
Over the years, rapid technological advancements have motivated organizations to implement efficient processes for supply chains (i.e., from design to manufacturing, logistics, and just-in-time delivery).
While these improvements help organizations increase efficiency and swiftly bring innovations to market, the rapid increase in scale, size, and complexity of supply chains has led to more frequent and sophisticated supply chain attacks.
The traditional methods of safeguarding supply chains (e.g., pre- and post-audit methodologies) are no longer adequate.

Problem Statement
=================
It is challenging to manage the compliance of products across end-to-end, global supply chains. 

Some of the fundamental security issues that face the supply chain ecosystem today are as follows:

1. A single product is composed of multiple sub-products coming from different suppliers. There is no agreed-upon standard to compose information from different producers.
2. No APIs are defined for automated publishing, retrieval, or independent verification of the information above.
3. Absence of decentralized globally interoperable transparency services to publish the supply chain data in a transparent manner.
4. Insufficient standards for independently verifying the presence of supply chain data in tamper-proof data stores.

A minimal, simple, and concise set of building blocks that interact in a standardized way will assure long-term accountability and interoperability for supply chain components throughout their lifecycles across architecturally diverse systems.

Goals
=====
Based on an input document on the architecture (draft-birkholz-scitt-architecture-00), the WG will:

1. Standardize the overall security flows for securing a software supply chain, covering the essential building blocks that make up the architecture, and
2. specify these building blocks, employing the existing work already done within other IETF WGs such as COSE WG, and IETF RATS WG, as appropriate.

The WG may refine the input document on the architecture in the process.

Non-Goals
=========
The WG does not:

1. make recommendations or suggestions on best practices on how to design the supply chain,
2. establish a universal/centralized registry for supply chain data,
3. try to prevent supply chain issuers from making false claims,
4. define specific implementation guidance on storage, query, or retrieval of supply chain statements, or
5. select a specific Bill of Materials (BOM) formats and metadata headers.

Program of Work
===============
The working group will develop standards supporting interoperable supply chain building blocks.
The main deliverables are as follows:

1. The WG will select (and potentially profile or augment) acceptable common identity format/formats that shall be used in the SCITT ecosystem. This will enable interoperability across geographical regions and also trace the identity chain seamlessly when a product comprises of multiple sub-products from multiple issuers. This includes a model of essential actors, such as the supply chain "issuer" (one which generates supply chain artifacts), and their duties in the ecosystem.

2. The WG will define the envelope and common schema for carrying supply chain claims/endorsements.

3. The WG will standardize the Transparent Registry requirements to generate homogeneity across multiple supply chains.

4. A standard format for authenticity data returned from the transparent registry, such as proof, etc. The standard will enable independent verification of supply chain claims at a (much) later point on multiple platforms across multiple geographical locations.

5. The WG will develop standards for auditing the supply chain claims that are introduced in the transparent registry. This will, in turn, generate audit claims (results of the audit) which can be introduced in the same registry. Audit information can be queried by supply chain consumers (end customers) before making critical business decisions.

6. The WG will develop standards that define the notarization process and outline the core functions/actions that a notary will perform in the supply chain ecosystem.

7. Standardize request-response interactions ("external API") and potentially other interaction models provided to various actors to interact with the supply chain ecosystem. This includes standardizing inter-component messages between supply chain building blocks to support easy reference implementations of SCITT building blocks by various organizations and easy industry-wide adaptation.
