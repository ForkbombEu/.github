<p align="center">
  <a href="https://forkbomb.solutions"><img src="./assets/hero.svg" width="100%" alt="Forkbomb: EUDI Wallet identity and Digital Product Passports, built on open, post-quantum ready cryptography"></a>
</p>

<p align="center">
  <a href="https://forkbomb.solutions"><b>forkbomb.solutions</b></a>
  &nbsp;·&nbsp; <a href="https://credimi.io">credimi.io</a>
  &nbsp;·&nbsp; <a href="https://didroom.com">didroom.com</a>
  &nbsp;·&nbsp; <a href="https://www.linkedin.com/company/forkbomb/">LinkedIn</a>
  &nbsp;·&nbsp; <a href="https://twitter.com/ForkbombEu">X</a>
  &nbsp;·&nbsp; <a href="mailto:info@forkbomb.eu">info@forkbomb.eu</a>
</p>

We build open-source software for the **European Digital Identity Wallet** and the **Digital Product Passport**: wallets, credential issuers and verifiers, the tools that prove they conform and interoperate, and passports that trace a product through its lifecycle.

Everything runs on one multiplatform cryptographic stack. Business logic is written in **Zencode**, an English-like language for cryptography, executed by the **Zenroom** virtual machine on servers, Android, iOS, browsers and embedded chips, with post-quantum algorithms (ML-DSA, ML-KEM) next to the classic ones.

Forkbomb B.V. was founded in October 2021 in Amsterdam as a spin-off of the [Dyne.org](https://dyne.org) foundation, where the Zenroom stack was born in EU research projects such as DECODE, REFLOW and the EBSI PCP.

## What we build

<table>
  <tr>
    <td width="50%" valign="top">
      <h3>Credimi</h3>
      <p><b>EUDI Wallet conformance and interoperability.</b> Test wallets, credential issuers and verifiers together against OpenID4VCI, OpenID4VP and the EUDI FCAF, on real devices, and keep the evidence of every run.</p>
      <p><a href="https://credimi.io">credimi.io</a> · <a href="https://docs.credimi.io">Docs</a> · <a href="https://atlas.credimi.io">EUDI Atlas</a> · <a href="https://trust-inspector.credimi.io">Trust Inspector</a> · <a href="https://github.com/ForkbombEu/credimi">Repository</a></p>
    </td>
    <td width="50%" valign="top">
      <h3>DIDroom</h3>
      <p><b>Open-source EUDI wallet stack.</b> Holder wallet and verifier apps for Android and iOS, OpenID4VCI and OpenID4VP issuer and verifier microservices, and an admin dashboard. SD-JWT VC, mDoc, W3C DID and VC, BBS+ and Coconut zero-knowledge credentials.</p>
      <p><a href="https://didroom.com">didroom.com</a> · <a href="https://github.com/ForkbombEu/wallet">Wallet</a> · <a href="https://github.com/ForkbombEu/verifier">Verifier</a> · <a href="https://github.com/ForkbombEu/DIDroom_microservices">Microservices</a></p>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h3>Digital Product Passport</h3>
      <p><b>Passports for complex supply chains.</b> Interfacer models products, materials and services on the ValueFlows ontology, identifies every actor with a W3C DID and anchors the passport on a blockchain so its history can be verified by third parties.</p>
      <p><a href="https://forkbomb.solutions/solution/interfacer-platform/">Interfacer</a> · <a href="https://github.com/interfacerproject/interfacer-dpp">interfacer-dpp</a> · <a href="https://github.com/interfacerproject/zenflows">zenflows</a></p>
    </td>
    <td width="50%" valign="top">
      <h3>Post-quantum and Zencode services</h3>
      <p><b>Crypto as readable contracts and REST APIs.</b> Hybrid post-quantum cryptography on server, mobile and browser; Zencode and Slangroom contracts served as microservices with ncr and deployed on AWS or Google Cloud with OpenTofu.</p>
      <p><a href="https://forkbombeu.github.io/pqspread/">PQSpread demo</a> · <a href="https://pqc.api.forkbomb.eu/docs">PQC API</a> · <a href="https://github.com/ForkbombEu/ncr">ncr</a> · <a href="https://apiroom.net">Apiroom IDE</a></p>
    </td>
  </tr>
</table>

<p align="center">
  <img src="./assets/stack.svg" width="100%" alt="The Forkbomb stack: a Zencode cryptography core on the Zenroom VM, Interfacer Digital Product Passports, DIDroom digital identity, and Credimi EUDI Wallet conformance, each with its open-source repositories">
</p>

## Standards we implement and test

<p align="center">
  <img src="./assets/standards.svg" width="100%" alt="OpenID4VCI, OpenID4VP, SD-JWT VC, ISO mDoc, EUDI ARF, EUDI FCAF, DCQL, W3C DID, W3C VC, ValueFlows DPP, Token Status List, ETSI TS 119 612, ML-DSA, ML-KEM, BBS, Coconut, KERI, ACDC and vLEI">
</p>

## Repositories

<details>
<summary><b>EUDI Wallet conformance and interoperability</b> · 12 repositories</summary>

| Repository | What it does |
| --- | --- |
| [`credimi`](https://github.com/ForkbombEu/credimi) | Automated conformance and interoperability testing platform and hub for EUDI and SSI wallets, credential issuers and verifiers (OpenID4VCI, OpenID4VP) |
| [`credimi-test-action`](https://github.com/ForkbombEu/credimi-test-action) | GitHub Action that runs Credimi pipelines in CI to test wallets, credential issuers and verifiers on every commit or pull request |
| [`eudi-conformance-evidence`](https://github.com/ForkbombEu/eudi-conformance-evidence) | Go module, CLI and web tool that resolves EUDI credential offers and presentation requests, with their metadata and JWT/JWS payloads, into structured conformance evidence |
| [`credimi-conformance-assessment`](https://github.com/ForkbombEu/credimi-conformance-assessment) | Go library, CLI and REST wrapper that generates Credimi conformance assessment reports from Temporal evidence and pipeline artifacts |
| [`eudi-trusted-lists-inspector`](https://github.com/ForkbombEu/eudi-trusted-lists-inspector) | CLI and API tool that tests EUDI LoTL and trusted lists for conformance with ETSI TS 119 602 and 119 612 |
| [`eudi-trusted-list-publisher`](https://github.com/ForkbombEu/eudi-trusted-list-publisher) | Publishes conformant and intentionally broken EUDI Trusted Lists to test how wallets, issuers and verifiers handle them |
| [`capture-status-list`](https://github.com/ForkbombEu/capture-status-list) | Mock Token Status List (TSL) server for EUDI Wallet conformance testing and debugging, serving JWT and CBOR/COSE CWT status lists |
| [`eudi-conformance-atlas`](https://github.com/ForkbombEu/eudi-conformance-atlas) | EUDI Trust & Conformance Atlas: static Eleventy site mapping EUDI Wallet law, ARF requirements, standards, trust work and conformance evidence |
| [`credimi-capture-wallet`](https://github.com/ForkbombEu/credimi-capture-wallet) | Uses the Credimi test issuer and verifier to obtain and present a PID while capturing wallet metadata, holder-binding and DPoP keys, and protocol calls |
| [`stepci-captured-runner`](https://github.com/ForkbombEu/stepci-captured-runner) | Bun CLI runner for StepCI YAML workflows with a capture plugin to transform and store captured values, used for Credimi test pipelines |
| [`avdctl`](https://github.com/ForkbombEu/avdctl) | CLI to manage Android emulator and iOS simulator lifecycles: AVD golden images, QCOW2-backed clones and parallel headless runs for CI |
| [`avdstream`](https://github.com/ForkbombEu/avdstream) | Real-time Android device screen streaming to the browser using scrcpy, v4l2loopback and MJPEG |

</details>

<details>
<summary><b>Digital identity</b> · 11 repositories</summary>

| Repository | What it does |
| --- | --- |
| [`wallet`](https://github.com/ForkbombEu/wallet) | DIDroom Wallet holder app for iOS and Android, built with Ionic and SvelteKit to store credentials and present them to DIDroom verifiers |
| [`verifier`](https://github.com/ForkbombEu/verifier) | DIDroom Verifier companion mobile app for verifying credentials presented from the DIDroom wallet |
| [`didroom-dashboard`](https://github.com/ForkbombEu/didroom-dashboard) | DIDroom dashboard (Signroom): EUDI-ARF/W3C-VC credential management and advanced electronic signature (*AdES) service based on Zenroom |
| [`DIDroom_microservices`](https://github.com/ForkbombEu/DIDroom_microservices) | DIDroom standalone microservices implementing OpenID4VC credential issuance on the Zenroom stack |
| [`didroom-components`](https://github.com/ForkbombEu/didroom-components) | Web components library for the DIDroom identity solution, built on the Custom Elements v1 standard for browsers and mobile |
| [`didroom-docs`](https://github.com/ForkbombEu/didroom-docs) | Documentation for DIDroom, the open-source SSI/EUDI wallet and issuer stack supporting OpenID4VCI, OpenID4VP and SD-JWT VC |
| [`mobile_zencode`](https://github.com/ForkbombEu/mobile_zencode) | Zencode and Slangroom contracts for DIDroom mobile components implementing OpenID4VCI and OpenID4VP on the Zenroom stack |
| [`CoconutIssuer`](https://github.com/ForkbombEu/CoconutIssuer) | Minimal Coconut credential issuer for DIDroom, based on the Coconut selective-disclosure credentials scheme |
| [`zencode-vc`](https://github.com/ForkbombEu/zencode-vc) | Zencode examples implementing W3C Verifiable Credentials and SD-JWT signature and verification with Zenroom |
| [`et-tu-cesr`](https://github.com/ForkbombEu/et-tu-cesr) | Go CLI that parses CESR streams used by KERI, ACDC and vLEI, printing JSON bodies and attachment block sizes |
| [`openid-vc-typescript-json-schema`](https://github.com/ForkbombEu/openid-vc-typescript-json-schema) | JSON Schemas and TypeScript definitions for OpenID4VCI (OpenID for Verifiable Credential Issuance), based on the editor's draft |

</details>

<details>
<summary><b>Digital Product Passport</b> · 3 repositories</summary>

| Repository | What it does |
| --- | --- |
| [`interfacerproject/interfacer-dpp`](https://github.com/interfacerproject/interfacer-dpp) | Microservice for managing Digital Product Passports |
| [`interfacerproject/zenflows`](https://github.com/interfacerproject/zenflows) | Resource-Event-Agent graph database governed by the ValueFlows vocabulary, the Interfacer DPP back-end |
| [`interfacerproject/zenflows-crypto`](https://github.com/interfacerproject/zenflows-crypto) | Zencode crypto functions for Zenflows |

</details>

<details>
<summary><b>Cryptography and Zencode services</b> · 8 repositories</summary>

| Repository | What it does |
| --- | --- |
| [`ncr`](https://github.com/ForkbombEu/ncr) | noˑcodeˑroom: no-code REST API server that exposes Zencode and Slangroom smart contracts as HTTP endpoints |
| [`twinroom`](https://github.com/ForkbombEu/twinroom) | CLI that runs Slangroom contracts written in Zencode, either embedded at build time or loaded from a folder |
| [`tf-ncr`](https://github.com/ForkbombEu/tf-ncr) | OpenTofu example deploying No-Code Room (NCR) Zencode microservices on Google Cloud and AWS, including PQC APIs |
| [`tf-pqcrypto-scripts`](https://github.com/ForkbombEu/tf-pqcrypto-scripts) | Post-quantum Zenroom scripts for ML-DSA-44 signing and verification, usable as a library or as microservices via NCR |
| [`pqspread`](https://github.com/ForkbombEu/pqspread) | Browser-based post-quantum file encryption and sharing |
| [`sd-jwt-zk`](https://github.com/ForkbombEu/sd-jwt-zk) | Zero-knowledge proof library for SD-JWT verifiable credential presentations, with selective disclosure and optional revocation checks |
| [`zkp-microservice`](https://github.com/ForkbombEu/zkp-microservice) | Zero-knowledge proof microservice (Longfellow, BBS) for generating and verifying proofs, written in Zencode and hosted with ncr |
| [`fouter`](https://github.com/ForkbombEu/fouter) | Go file-based router that discovers .slang files from embedded and local filesystems to serve Slangroom scripts as routes |

</details>

## Research and EU projects

Our software grew out of, and keeps feeding, European research and large-scale pilots:

- **[WE BUILD](https://forkbomb.solutions/project/we-build/)**: large-scale pilot for a trusted digital business identity ecosystem on the EUDI Wallet framework, where Credimi provides conformance and interoperability testing.
- **[EBSI PCP](https://forkbomb.solutions/project/ebsi-pcp/)**, **[DECODE](https://forkbomb.solutions/project/decode/)** and **[REFLOW](https://forkbomb.solutions/project/reflow/)**: the projects where the Zenroom stack was designed and proven.
- **[INTERFACER](https://forkbomb.solutions/project/interfacer/)** and **[CLOSER](https://forkbomb.solutions/project/closer/)**: Digital Product Passports and circular supply chains, down to critical raw materials for chips.

Development of DIDroom and Credimi is supported by [NGI TRUSTCHAIN](https://trustchain.ngi.eu/), and DIDroom by [NGI Sargasso](https://ngisargasso.eu/), with financial support from the European Commission's Next Generation Internet programme.

## Work with us

We design, build and customise solutions with companies and institutions: EUDI Wallet credentials for health and retail services, product passports for manufacturing, cryptographic oracles and post-quantum cryptography. See the [use cases](https://forkbomb.solutions/use-cases/) or write to [info@forkbomb.eu](mailto:info@forkbomb.eu).

<sub>Forkbomb B.V. · Haparandadam 7-A1, 1013AK Amsterdam, the Netherlands</sub>
