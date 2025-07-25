## SWIDs

A Spatial Web Identifier (SWID) is any [[ref: DID]] which fulfills the following two requirements:

1. The DID and its associated DID document MUST be conformant with the [[spec: DID-CORE]]
specification.

2. The associated DID document MUST be a conformant [SWID Document](#swid-documents).

There is no direct restriction for SWIDs with regard to which DID method they use, as long as the two requirements
above are fulfilled. Different DID methods have different properties with regard to decentralization, scalability,
cost, etc. Depending on the use case, some DID methods may be more suited than others due to such properties.

Note that some DID methods have technical limitations that make them unsuitable for SWIDs. For example, the
`did:key` DID method does not support service endpoints in DID documents, therefore this DID method cannot be used
for SWIDs.

Note that one DID method - `did:swid` - has been specifically designed to meet the requirements
of SWIDs for the Spatial Web. See [[spec: DID-SWID]] for the specification.

### Example SWIDs

The following are compliant SWIDs using different DID methods:

- `did:web:did-web.dev.godiddy.com:575dcb04-9219-49a8-a6ac-0f982ee17438`
- `did:cheqd:testnet:348e4b40-dff4-4f07-987b-833e3f6e01be`
- `did:indy:danube:MafjMzJVnX7p5FEv47k8hi`
- `did:ethr:sepolia:0x0349de79b43afff92e1db0806272aacc3bd644f0b5622d2dfa310f2aa7180be3f2`
- `did:ebsi:zeUucvX2jE79e75xXSxf9S2`
- `did:ion:test:EiBBuOWqiR-KD5KByXG8hQ2vycAmT_k3o0agsA1Ntd2guA`

They can be resolved using DID Resolution tools such as https://dev.uniresolver.io/ or https://godiddy.com/.
