# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]
# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [0.29.0](https://github.com/orthecreedence/rasn/compare/rasn-derive-v0.28.4...rasn-derive-v0.29.0) - 2026-01-22

### Added

- #[derive(Decode)] changes to make generics more robust ([#515](https://github.com/orthecreedence/rasn/pull/515))
- support multi-field tuple-structs with delegate if other types are ([#436](https://github.com/orthecreedence/rasn/pull/436))
- [**breaking**] Remove option_type ([#329](https://github.com/orthecreedence/rasn/pull/329))
- Constraint utilities, const default, more const functions ([#321](https://github.com/orthecreedence/rasn/pull/321))

### Fixed

- Sanitize field attributes when expanding Decode and Encode ([#509](https://github.com/orthecreedence/rasn/pull/509))
- use full paths for field encode/decode, remove nightly CI ([#499](https://github.com/orthecreedence/rasn/pull/499))
- *(OER/PER)* detect choice type always correctly on explicit prefix ([#479](https://github.com/orthecreedence/rasn/pull/479))
- improve constraint performance and bounded intersection ([#440](https://github.com/orthecreedence/rasn/pull/440))
- *(derive)* use `const` blocks and add generic bounds when generating an enum's `AsnType` impl ([#398](https://github.com/orthecreedence/rasn/pull/398))
- cleanup some unnecessary dependencies ([#362](https://github.com/orthecreedence/rasn/pull/362))
- Don't override generics impl in proc-macros on encode impl ([#354](https://github.com/orthecreedence/rasn/pull/354))
- decoding of extended fields in sequence in BER ([#351](https://github.com/orthecreedence/rasn/pull/351))
- Run clippy and rustdoc only on stable channel in CI ([#342](https://github.com/orthecreedence/rasn/pull/342))
- macros: include license texts in the packaged crate ([#330](https://github.com/orthecreedence/rasn/pull/330))
- [**breaking**] Remove Tag and TagTree from module root
- *(macro)* recognize option references ([#219](https://github.com/orthecreedence/rasn/pull/219))
- *(macros)* handle negative discriminants
- fix explicit prefix decode & encode for macros
- fix
- fix missing pieces for derive

### Other

- release v0.28.4 ([#524](https://github.com/orthecreedence/rasn/pull/524))
- release v0.28.3 ([#517](https://github.com/orthecreedence/rasn/pull/517))
- release v0.28.2 ([#512](https://github.com/orthecreedence/rasn/pull/512))
- Fixing #[derive(Decode)] issue where generics were not passed into the decode op, causing an error when deriving/compiling ([#513](https://github.com/orthecreedence/rasn/pull/513))
- release v0.28.1 ([#510](https://github.com/orthecreedence/rasn/pull/510))
- release v0.27.5 ([#500](https://github.com/orthecreedence/rasn/pull/500))
- release v0.27.4 ([#498](https://github.com/orthecreedence/rasn/pull/498))
- release v0.27.3 ([#494](https://github.com/orthecreedence/rasn/pull/494))
- release v0.27.2 ([#490](https://github.com/orthecreedence/rasn/pull/490))
- release v0.27.1 ([#481](https://github.com/orthecreedence/rasn/pull/481))
- clippy pendantic fixes ([#444](https://github.com/orthecreedence/rasn/pull/444))
- release v0.27.0 ([#470](https://github.com/orthecreedence/rasn/pull/470))
- *(ci)* fix clippy lints
- release v0.26.6 ([#464](https://github.com/orthecreedence/rasn/pull/464))
- release v0.26.5 ([#463](https://github.com/orthecreedence/rasn/pull/463))
- release v0.26.4 ([#460](https://github.com/orthecreedence/rasn/pull/460))
- release v0.26.3 ([#456](https://github.com/orthecreedence/rasn/pull/456))
- release v0.26.2 ([#439](https://github.com/orthecreedence/rasn/pull/439))
- release v0.26.1 ([#434](https://github.com/orthecreedence/rasn/pull/434))
- release v0.26.0 ([#423](https://github.com/orthecreedence/rasn/pull/423))
- Improve constraint compiler errors ([#428](https://github.com/orthecreedence/rasn/pull/428))
- Ignore .profraw, remove related ([#424](https://github.com/orthecreedence/rasn/pull/424))
- Add decoding iterator, decode_with_remainder, clippy fixes ([#421](https://github.com/orthecreedence/rasn/pull/421))
- release v0.25.1 ([#422](https://github.com/orthecreedence/rasn/pull/422))
- Fixes librasn/rasn#418. Add support for explict tags and default values to encode correctly ([#419](https://github.com/orthecreedence/rasn/pull/419))
- release v0.24.1 ([#411](https://github.com/orthecreedence/rasn/pull/411))
- Feat/xml encoding rules ([#416](https://github.com/orthecreedence/rasn/pull/416))
- release v0.23.1 ([#409](https://github.com/orthecreedence/rasn/pull/409))
- release v0.22.3 ([#402](https://github.com/orthecreedence/rasn/pull/402))
- release v0.22.2 ([#401](https://github.com/orthecreedence/rasn/pull/401))
- Better error messages for derives ([#400](https://github.com/orthecreedence/rasn/pull/400))
- release v0.22.1 ([#380](https://github.com/orthecreedence/rasn/pull/380))
- OER: remove nom usage, improve errors ([#384](https://github.com/orthecreedence/rasn/pull/384))
- release v0.21.1 ([#371](https://github.com/orthecreedence/rasn/pull/371))
- [**breaking**] Add lifetime for `encoder` trait and add allocation improvements based on that (OER) ([#370](https://github.com/orthecreedence/rasn/pull/370))
- OER: improve decoding presence tracking ([#375](https://github.com/orthecreedence/rasn/pull/375))
- rasn-derive-impl version ([#372](https://github.com/orthecreedence/rasn/pull/372))
- Make constraints explicitly constant and evaluated in compile time & move some computation there (OER/PER) ([#318](https://github.com/orthecreedence/rasn/pull/318))
- release v0.21.0 ([#367](https://github.com/orthecreedence/rasn/pull/367))
- Extract proc macro into own crate ([#364](https://github.com/orthecreedence/rasn/pull/364))
- Optimize field presence tracking of default/optional/extended fields ([#324](https://github.com/orthecreedence/rasn/pull/324))
- Disallow structs without fields for a `set` ([#352](https://github.com/orthecreedence/rasn/pull/352))
- update dependencies
- release v0.20.2 ([#343](https://github.com/orthecreedence/rasn/pull/343))
- Update to syn2 ([#345](https://github.com/orthecreedence/rasn/pull/345))
- release ([#332](https://github.com/orthecreedence/rasn/pull/332))
- clippy fixes
- release ([#320](https://github.com/orthecreedence/rasn/pull/320))
- release ([#316](https://github.com/orthecreedence/rasn/pull/316))
- Update itertools to 0.13, update Cargo.lock
- release ([#267](https://github.com/orthecreedence/rasn/pull/267))
- Fix error name regression introduced in a75b26b ([#285](https://github.com/orthecreedence/rasn/pull/285))
- release ([#264](https://github.com/orthecreedence/rasn/pull/264))
- *(ber)* don't allocate `2 + N` `BigInt`s when parsing OIDs ([#263](https://github.com/orthecreedence/rasn/pull/263))
- release ([#248](https://github.com/orthecreedence/rasn/pull/248))
- Remove `backtraces` from `rasn`'s `default` feature ([#247](https://github.com/orthecreedence/rasn/pull/247))
- release ([#241](https://github.com/orthecreedence/rasn/pull/241))
- Feat/identifier annotation ([#239](https://github.com/orthecreedence/rasn/pull/239))
- Add clippy and fix reported issues ([#234](https://github.com/orthecreedence/rasn/pull/234))
- release ([#231](https://github.com/orthecreedence/rasn/pull/231))
- *(macros)* Treat Unit Structs as ASN.1 NULL ([#227](https://github.com/orthecreedence/rasn/pull/227))
- Fix calling the specified default fn
- Add default_initializer_fn optimisation
- release ([#215](https://github.com/orthecreedence/rasn/pull/215))
- release ([#203](https://github.com/orthecreedence/rasn/pull/203))
- Fix PER ObjectIdentifier, Alignment for Choice index encoding ([#202](https://github.com/orthecreedence/rasn/pull/202))
- release ([#196](https://github.com/orthecreedence/rasn/pull/196))
- Add `Option<T::EXTENDED_VARIANTS>` for Choice, clippy cleanup for relevant macros ([#200](https://github.com/orthecreedence/rasn/pull/200))
- Feature/jer ([#187](https://github.com/orthecreedence/rasn/pull/187))
- Field_error improved, Boxed error `kind`, explicit naming also for `DecodeErrorKind` ([#197](https://github.com/orthecreedence/rasn/pull/197))
- run cargo fmt
- release ([#189](https://github.com/orthecreedence/rasn/pull/189))
- Shared error module ([#164](https://github.com/orthecreedence/rasn/pull/164))
- release ([#182](https://github.com/orthecreedence/rasn/pull/182))
- Add CI check for formatted files and reformat source ([#181](https://github.com/orthecreedence/rasn/pull/181))
- release ([#178](https://github.com/orthecreedence/rasn/pull/178))
- four uper issues ([#177](https://github.com/orthecreedence/rasn/pull/177))
- release ([#173](https://github.com/orthecreedence/rasn/pull/173))
- Fix/issue 165 ([#172](https://github.com/orthecreedence/rasn/pull/172))
- release ([#160](https://github.com/orthecreedence/rasn/pull/160))
- Gensym field names ([#166](https://github.com/orthecreedence/rasn/pull/166))
- Delegate newtype EOC ([#163](https://github.com/orthecreedence/rasn/pull/163))
- Fix Result scoping ([#162](https://github.com/orthecreedence/rasn/pull/162))
- Fix/infinite recursion ([#157](https://github.com/orthecreedence/rasn/pull/157))
- Fix/constrained extension ([#156](https://github.com/orthecreedence/rasn/pull/156))
- Use workspace for macros
- Fix Clippy warnings ([#132](https://github.com/orthecreedence/rasn/pull/132))
- Release 0.8.2
- bump macros
- release ([#122](https://github.com/orthecreedence/rasn/pull/122))
- Add constraints to PKIX
- clippy
- Implement Unpacked Encoding Rules (UPER)
- Release 0.6.0
- Convert `Result` in macros to `core::result::Result`
- Release 0.5.2
- fmt
- Account for every possible position of #[tag(explicit)]
- Release 0.5.1
- fmt
- More explicit prefix macro fixes
- Update deps
- Fix explicit tag parsing
- Release 0.5.0
- Replace static_assertions with 1.57 const assert
- format macros
- Fix default parsing and TAG_TREE for SEQUENCE variants
- Add support for Kerberos & OCSP, and fix explicit tag codegen
- Use ty directly instead of inference in macro default
- Release 0.4.0
- Clippy fixes and formatting
- misc improvements
- Make is_unique an associated method
- refactor field encoding and decoding to be more DRY and use default attribute
- Improve error message more
- Add better error messages for fields and choices
- Add support for SET and explicit tags to macros
- rm dbg
- Ensure explict prefix encodes constructed values correctly. Closes #35
- Fix option decoding
- Fix derive codegen
- Move tagging inside the trait implementations
- Revert "Make field encoding generation more DRY"
- Make field encoding generation more DRY
- Fix proc macro struct field codecs
- Improved README, and automatic_tags
- Fix tag detection in newtype wrappers
- Fix tagged choice variants
- Small improvements to error messages, and clean up newly-dead tag constant defs ([#22](https://github.com/orthecreedence/rasn/pull/22))
- Add proc macros and add trap message test
- Add docs and tidy up
- Create TagTree and refactor Tag validation and CHOICE decoding
- Release 0.3.0
- Add more documentation
- Implement MIB-II, Add #[rasn(delegate)] and #[rasn(default)]
- Add support for generics in proc macro
- Improved various aspects of rasn-macros
- Add Oid and use const generics for tag
- Release 0.2.1
- Add a new `#[rasn(choice)]` field attribute
- remove old dependency
- Release 0.2.0
- Add metadata to macros crate
- more docs
- Add docs and fix constructed encoding for strings
- Implement automatic tagging
- Implement tagging attribute for all valid positions
- Refactor tests, add option impl, add docs
- split up proc macro exports
- Add static asserts and time types
- Fix more macro bugs and make open type complete
- fuzzing fixes
- fmt
- Implemented initial support for choice enums
- Add initial macro support for structs and enums

## [0.27.0](https://github.com/librasn/rasn/compare/rasn-derive-v0.26.6...rasn-derive-v0.27.0) - 2025-06-19

### Fixed

- *(OER/PER)* detect choice type always correctly on explicit prefix ([#479](https://github.com/librasn/rasn/pull/479))

### Other

- *(ci)* fix clippy lints

## [0.26.2](https://github.com/librasn/rasn/compare/rasn-derive-v0.26.1...rasn-derive-v0.26.2) - 2025-04-17

### Added

- support multi-field tuple-structs with delegate if other types are ([#436](https://github.com/librasn/rasn/pull/436))

### Fixed

- improve constraint performance and bounded intersection ([#440](https://github.com/librasn/rasn/pull/440))

## [0.22.2](https://github.com/librasn/rasn/compare/rasn-derive-v0.22.1...rasn-derive-v0.22.2) - 2025-01-05

### Other

- Better error messages for derives ([#400](https://github.com/librasn/rasn/pull/400))

## [0.21.0](https://github.com/librasn/rasn/compare/rasn-derive-v0.20.2...rasn-derive-v0.21.0) - 2024-11-12

### Fixed

- cleanup some unnecessary dependencies ([#362](https://github.com/librasn/rasn/pull/362))
- Don't override generics impl in proc-macros on encode impl ([#354](https://github.com/librasn/rasn/pull/354))
- decoding of extended fields in sequence in BER ([#351](https://github.com/librasn/rasn/pull/351))

### Other

- Extract proc macro into own crate ([#364](https://github.com/librasn/rasn/pull/364))
- Optimize field presence tracking of default/optional/extended fields ([#324](https://github.com/librasn/rasn/pull/324))
- Disallow structs without fields for a `set` ([#352](https://github.com/librasn/rasn/pull/352))
- update dependencies

## [0.20.2](https://github.com/librasn/rasn/compare/rasn-derive-v0.20.1...rasn-derive-v0.20.2) - 2024-10-18

### Fixed

- Run clippy and rustdoc only on stable channel in CI ([#342](https://github.com/librasn/rasn/pull/342))

### Other

- Update to syn2 ([#345](https://github.com/librasn/rasn/pull/345))

## [0.19.0](https://github.com/librasn/rasn/compare/rasn-derive-v0.18.0...rasn-derive-v0.19.0) - 2024-09-22

### Other

- clippy fixes

## [0.18.0](https://github.com/librasn/rasn/compare/rasn-derive-v0.17.3...rasn-derive-v0.18.0) - 2024-09-17

### Added

- [**breaking**] Remove option_type ([#329](https://github.com/librasn/rasn/pull/329))
- Constraint utilities, const default, more const functions ([#321](https://github.com/librasn/rasn/pull/321))

### Fixed

- macros: include license texts in the packaged crate ([#330](https://github.com/librasn/rasn/pull/330))
- [**breaking**] Remove Tag and TagTree from module root

## [0.17.3](https://github.com/librasn/rasn/compare/rasn-derive-v0.17.2...rasn-derive-v0.17.3) - 2024-09-12

### Other

- Update itertools to 0.13, update Cargo.lock

## [0.16.0](https://github.com/librasn/rasn/compare/rasn-derive-v0.15.3...rasn-derive-v0.16.0) - 2024-07-17

### Other
- Fix error name regression introduced in a75b26b ([#285](https://github.com/librasn/rasn/pull/285))

## [0.15.3](https://github.com/librasn/rasn/compare/rasn-derive-v0.15.2...rasn-derive-v0.15.3) - 2024-06-14

### Other
- *(ber)* don't allocate `2 + N` `BigInt`s when parsing OIDs ([#263](https://github.com/librasn/rasn/pull/263))

## [0.15.0](https://github.com/librasn/rasn/compare/rasn-derive-v0.14.0...rasn-derive-v0.15.0) - 2024-05-17

### Other
- Remove `backtraces` from `rasn`'s `default` feature ([#247](https://github.com/librasn/rasn/pull/247))

## [0.14.0](https://github.com/librasn/rasn/compare/rasn-derive-v0.13.1...rasn-derive-v0.14.0) - 2024-04-04

### Other
- Feat/identifier annotation ([#239](https://github.com/librasn/rasn/pull/239))

## [0.12.6](https://github.com/librasn/rasn/compare/rasn-derive-v0.12.5...rasn-derive-v0.12.6) - 2024-03-09

### Other
- *(macros)* Treat Unit Structs as ASN.1 NULL ([#227](https://github.com/librasn/rasn/pull/227))
- Fix calling the specified default fn
- Add default_initializer_fn optimisation

## [0.12.5](https://github.com/librasn/rasn/compare/rasn-derive-v0.12.4...rasn-derive-v0.12.5) - 2024-02-02

### Fixed
- *(macro)* recognize option references ([#219](https://github.com/librasn/rasn/pull/219))

## [0.12.1](https://github.com/XAMPPRocky/rasn/compare/rasn-derive-v0.12.0...rasn-derive-v0.12.1) - 2023-11-14

### Other
- Fix PER ObjectIdentifier, Alignment for Choice index encoding ([#202](https://github.com/XAMPPRocky/rasn/pull/202))

## [0.12.0](https://github.com/XAMPPRocky/rasn/compare/rasn-derive-v0.11.1...rasn-derive-v0.12.0) - 2023-11-12

### Fixed
- *(macros)* handle negative discriminants

### Other
- Add `Option<T::EXTENDED_VARIANTS>` for Choice, clippy cleanup for relevant macros ([#200](https://github.com/XAMPPRocky/rasn/pull/200))
- Feature/jer ([#187](https://github.com/XAMPPRocky/rasn/pull/187))
- Field_error improved, Boxed error `kind`, explicit naming also for `DecodeErrorKind` ([#197](https://github.com/XAMPPRocky/rasn/pull/197))
- run cargo fmt

## [0.11.0](https://github.com/XAMPPRocky/rasn/compare/rasn-derive-v0.10.6...rasn-derive-v0.11.0) - 2023-10-28

### Other
- Shared error module ([#164](https://github.com/XAMPPRocky/rasn/pull/164))

## [0.10.6](https://github.com/XAMPPRocky/rasn/compare/rasn-derive-v0.10.5...rasn-derive-v0.10.6) - 2023-10-26

### Other
- Add CI check for formatted files and reformat source ([#181](https://github.com/XAMPPRocky/rasn/pull/181))

## [0.10.4](https://github.com/XAMPPRocky/rasn/compare/rasn-derive-v0.10.3...rasn-derive-v0.10.4) - 2023-10-16

### Other
- four uper issues ([#177](https://github.com/XAMPPRocky/rasn/pull/177))

## [0.10.2](https://github.com/XAMPPRocky/rasn/compare/rasn-derive-v0.10.1...rasn-derive-v0.10.2) - 2023-10-10

### Other
- Fix/issue 165 ([#172](https://github.com/XAMPPRocky/rasn/pull/172))

## [0.10.0](https://github.com/XAMPPRocky/rasn/compare/rasn-derive-v0.9.5...rasn-derive-v0.10.0) - 2023-10-03

### Other
- Gensym field names ([#166](https://github.com/XAMPPRocky/rasn/pull/166))
- Delegate newtype EOC ([#163](https://github.com/XAMPPRocky/rasn/pull/163))
- Fix Result scoping ([#162](https://github.com/XAMPPRocky/rasn/pull/162))
- Fix/infinite recursion ([#157](https://github.com/XAMPPRocky/rasn/pull/157))
- Fix/constrained extension ([#156](https://github.com/XAMPPRocky/rasn/pull/156))

## [0.6.1](https://github.com/XAMPPRocky/rasn/compare/rasn-derive-v0.6.0...rasn-derive-v0.6.1) - 2023-07-11

### Other
- Add constraints to PKIX
- clippy
- Implement Unpacked Encoding Rules (UPER)
