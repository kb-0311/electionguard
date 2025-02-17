# ElectionGuard Official Specifications 

The official versions of the ElectionGuard Specifications are listed below and stand as the primary source of reference when discussing the [ElectionGuard Specification]. Each version includes a [badge] that can be used to quickly display which versions are supported or used by products following the specification. 


Version | Specification                                  | Recommended      | Badge       
:------ |:-----------------------------------------------|:----------------:| :-----------
2.0     | _Unreleased_                                   |                  | ![Version 2.0][badge-2.0]
1.0     | [:material-download: Download][spec-1.0]       | :material-check: | ![Version 1.0][badge-1.0]
0.95    | [:material-download: Download][spec-0.95]      | :material-check: | ![Version 0.95][badge-0.95]
0.85    | [:material-download: Download][spec-0.85]      |                  | ![Version 0.85][badge-0.85]


### Release Notes

#### v1.0

_Updates from previous version_

- The large prime p and corresponding cofactor r were changed to correctly match the result of the process for the derivation of the prime.
- The equations for generating proofs of ballot correctness have been optimized.
- Auxiliary keys have been eliminated in favor of using the existing keys for both ordinary and exponential ElGamal encryption.
- A more flexible structure of ballot chaining has been introduced to allow for non-linear chaining or no chaining at all.
- Smaller parameters suitable for testing are included.
- The election record of this version should match that of the prior v0.95 and therefore require no verifier changes (with the exception of using the corrected prime).

#### v0.95

_Updates from previous version_

- The large prime p and corresponding cofactor r were changed to move the prime p further from 2^4096.
- A section specifically about writing verifiers was added.
- Various small clarifications and corrections were included.
 

#### v0.85

- Initial public release of specification for ElectionGuard

!!! warning "ElectionGuard Web Specification"
    The [web version] is being constructed by the open source community for the convenience of web viewing. However, it is incomplete at this time and should not be used for reference purposes. If you need a complete reference, refer to the official specifications.



<!-- Links -->
[ElectionGuard Specification]: ../overview/Glossary/#electionguard-specification
[badge]: ../develop/Badges/
[web version]: ./web/1_Overview.md

[badge-2.0]: https://img.shields.io/badge/🗳%20ElectionGuard%20Specification-v2.0-yellow

[badge-1.0]: https://img.shields.io/badge/🗳%20ElectionGuard%20Specification-v1.0-green
[spec-1.0]: https://github.com/microsoft/electionguard/releases/download/v1.0/EG_spec_v1_0.pdf "Election Guard Specification 1.0"

[badge-0.95]: https://img.shields.io/badge/🗳%20ElectionGuard%20Specification-v0.95-green
[spec-0.95]: https://github.com/microsoft/electionguard/releases/download/v0.95.0/EG_spec_v0_95.pdf "Election Guard Specification 0.95"

[badge-0.85]: https://img.shields.io/badge/🗳%20ElectionGuard%20Specification-v0.85-green
[spec-0.85]: https://github.com/microsoft/electionguard/releases/download/v0.85.0/EG_spec_V0_85.pdf "Election Guard Specification 0.85"

