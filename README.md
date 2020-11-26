# ArStore

#### A framework allowing organizations to adopt ArWeave incrementally for object storage. 

---

Let's take, for example, a Culturally Important Magazine. Currently, their editors use A Boring CMS to manage content and they persist their data on a cloud-based network. Increasingly, murmurs have been spreading amongst literary circles about government activity around censorship. One of the younger guys on staff brings something called ArWeave to the attention of the CTO, who’s immediately excited by the notion of decentralization and data permanence.  

She looks into it a bit. ArWeave is without question exciting but the ecosystem is still small. She notices the apps are promising but incontrovertibly less mature than what she's used to. She also only faintly knows how a blockchain works and fears the risks inherent to embracing a new technology. She can’t help but feel wary of the cognitive barriers w/ re: to the mechanics/implementation. Right away, she knows they’re not ready to bring their whole operation over to the permaweb and wishes there were a simple, configurable Boring CMS plugin instead. At the point of content-submission, she would love it if editors were able to tick a box and upload sensitive works to ArWeave for safe-keeping.

---

The approach I propose here is to build:

1. A UI to operate upon data, to faciliate sign-ups, and to manage account settings. It would allow users to create their organization, generate schemas to describe the various shapes of their data (more of a stretch goal: schemas could be used to validate against before committing data), as well as serving a kind of simple CRUD interace for users to manage their data. The UI would be comparable to a headless CMS.

2. An API/library to handle the legwork. It would offer a dumbed-down interface relative to the current Arweave HTTP API in the hopes of encapsulating as much as possible of the complexity necessary to interface with the chain, leveraging account settings originally configured via the UI to prime dev-facing convenience functions. The library could be used to build plugins, adapaters, etc.

Quickly, roughly:

![library](https://github.com/duncanlettuce/ArStore/blob/concept/library.png)

---

![flowchart](https://github.com/duncanlettuce/ArStore/blob/concept/flowchart.png)

---

ArWeave as well as blockchain-based tech in general are still very new to me so, questions:

1. This concept is pretty basic/foundational; is it already spoken for by someone else?
2. In order to create a library, as sketched above, that would serve to access the HTTP API, is it as simple as making wrappers around the official ArWeave SDKs?

*I believe it's particularly vital to bring this ease of use to those who would otherwise pass on ArWeave. I strongly suspect that reducing the magnitude of complexity in ArWeave's current implementation workflows (making it "dead simple") would contribute to a noticeable increase in traction not only with new Arweave users but with Arweave builders/developers. There are obviously significant challenges, namely in the general breadth of the project. Successfully executing this concept would require a dedicated team and a strong commitment to growth.*
