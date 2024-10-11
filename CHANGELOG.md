# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [0.13.0](https://github.com/EmbarkStudios/pprof-rs/releases/tag/v0.13.0) - 2024-10-11

### Added

- Fix and cover tests for target x86_64-unknown-linux-musl  ([#140](https://github.com/EmbarkStudios/pprof-rs/pull/140))

### Fixed

- renaming
- remove protobuf crate
- check if ptr is valid in validate
- rename crate in examples
- use T aligned pointer in TempFdArray
- handle potentially unaligned frame pointer ([#217](https://github.com/EmbarkStudios/pprof-rs/pull/217))
- fix memory leak in collector ([#84](https://github.com/EmbarkStudios/pprof-rs/pull/84))
- fix clippy error ([#52](https://github.com/EmbarkStudios/pprof-rs/pull/52))
- fix incorrect inline functions ([#50](https://github.com/EmbarkStudios/pprof-rs/pull/50))
- fix test
- fix example import ([#25](https://github.com/EmbarkStudios/pprof-rs/pull/25))
- fix bugs caused by link test all the time
- fix bugs in TempFdArray
- fix bug: buffer in TempFdArray should be sliced when iter around it
- fix bug: malloc shouldn't be used in signal handler
- fix cargo warning

### Other

- Update release-plz.yaml
- Update rust.yml
- Update rust.yml
- move cpu logs to debug
- update prost file
- fix benches
- fix lints
- update CI minimum to 1.81.0
- Create release-plz.yaml
- update dependencies
- Rename to pprof2, update MSRV
- Bump version to v0.13.0 ([#226](https://github.com/EmbarkStudios/pprof-rs/pull/226))
- Update `prost`, `prost-derive` and `prost-build` to `0.12` ([#223](https://github.com/EmbarkStudios/pprof-rs/pull/223))
- Fix clippy errors ([#224](https://github.com/EmbarkStudios/pprof-rs/pull/224))
- Fix CI for 1.64.0 ([#225](https://github.com/EmbarkStudios/pprof-rs/pull/225))
- Bump version to v0.12.1 ([#220](https://github.com/EmbarkStudios/pprof-rs/pull/220))
- Change sc_pc to __pc for loongarch64 ([#218](https://github.com/EmbarkStudios/pprof-rs/pull/218))
- Bump version to v0.12.0 ([#215](https://github.com/EmbarkStudios/pprof-rs/pull/215))
- Support freebsd ([#213](https://github.com/EmbarkStudios/pprof-rs/pull/213))
- update to criterion 0.5 ([#212](https://github.com/EmbarkStudios/pprof-rs/pull/212))
- hide `perf_signal_handler` frames on macOS ([#207](https://github.com/EmbarkStudios/pprof-rs/pull/207))
- Splitting profile_proto example ([#208](https://github.com/EmbarkStudios/pprof-rs/pull/208))
- Bump the symbolic-demangle to 12.1 ([#205](https://github.com/EmbarkStudios/pprof-rs/pull/205))
- Correct required-features for profile_proto example ([#206](https://github.com/EmbarkStudios/pprof-rs/pull/206))
- Fix build for aarch64-linux-android ([#202](https://github.com/EmbarkStudios/pprof-rs/pull/202))
- Bump the MSRV to 1.64.0 ([#204](https://github.com/EmbarkStudios/pprof-rs/pull/204))
- bump version to 0.11.1 ([#199](https://github.com/EmbarkStudios/pprof-rs/pull/199))
- use globally shared pipe to validate memory ([#198](https://github.com/EmbarkStudios/pprof-rs/pull/198))
- update the prost generated file and remove malloc_free ([#188](https://github.com/EmbarkStudios/pprof-rs/pull/188))
- Update nix requirement from 0.24 to 0.26 ([#179](https://github.com/EmbarkStudios/pprof-rs/pull/179))
- Add loongarch64 support ([#174](https://github.com/EmbarkStudios/pprof-rs/pull/174))
- add riscv arch ([#169](https://github.com/EmbarkStudios/pprof-rs/pull/169))
- Improve prost file format ([#175](https://github.com/EmbarkStudios/pprof-rs/pull/175))
- Bump version to v0.11.0 ([#173](https://github.com/EmbarkStudios/pprof-rs/pull/173))
- Update symbolic-demangle requirement from 9.0 to 10.1 ([#170](https://github.com/EmbarkStudios/pprof-rs/pull/170))
- Only do per-frame-blocklist-check when frame-pointer is enabled ([#172](https://github.com/EmbarkStudios/pprof-rs/pull/172))
- Restart syscalls interrupted by SIGPROF when possible ([#167](https://github.com/EmbarkStudios/pprof-rs/pull/167))
- update prost 0.11 ([#166](https://github.com/EmbarkStudios/pprof-rs/pull/166))
- Update criterion requirement from 0.3 to 0.4 ([#163](https://github.com/EmbarkStudios/pprof-rs/pull/163))
- Bump version to v0.10.1 ([#162](https://github.com/EmbarkStudios/pprof-rs/pull/162))
- Bump version to v0.10.1 ([#161](https://github.com/EmbarkStudios/pprof-rs/pull/161))
- Increase the max supported stack depth to 128 ([#159](https://github.com/EmbarkStudios/pprof-rs/pull/159))
- ignore prost mod and fix clippy warning ([#160](https://github.com/EmbarkStudios/pprof-rs/pull/160))
- Bump version to v0.10.0 ([#146](https://github.com/EmbarkStudios/pprof-rs/pull/146))
- Make clippy happy in all targets ([#144](https://github.com/EmbarkStudios/pprof-rs/pull/144))
- Update symbolic-demangle requirement from 8.0 to 9.0 ([#137](https://github.com/EmbarkStudios/pprof-rs/pull/137))
- Adds timing info to each sample ([#133](https://github.com/EmbarkStudios/pprof-rs/pull/133))
- Export UnresolvedReport ([#132](https://github.com/EmbarkStudios/pprof-rs/pull/132))
- Optimize mutually exclusive features ([#130](https://github.com/EmbarkStudios/pprof-rs/pull/130))
- Bump version to 0.9.1 ([#129](https://github.com/EmbarkStudios/pprof-rs/pull/129))
- Protect errno ([#128](https://github.com/EmbarkStudios/pprof-rs/pull/128))
- bump version to v0.9.0 ([#124](https://github.com/EmbarkStudios/pprof-rs/pull/124))
- add fs feature ([#125](https://github.com/EmbarkStudios/pprof-rs/pull/125))
- Update nix to 0.24, limit features ([#121](https://github.com/EmbarkStudios/pprof-rs/pull/121))
- Unwind through frame pointer ([#116](https://github.com/EmbarkStudios/pprof-rs/pull/116))
- Bump version to 0.8 ([#118](https://github.com/EmbarkStudios/pprof-rs/pull/118))
- Update prost requirement from 0.9 to 0.10 ([#115](https://github.com/EmbarkStudios/pprof-rs/pull/115))
- Update prost-build requirement from 0.9 to 0.10 ([#114](https://github.com/EmbarkStudios/pprof-rs/pull/114))
- Update prost-derive requirement from 0.9 to 0.10 ([#113](https://github.com/EmbarkStudios/pprof-rs/pull/113))
- Update Readme to fix the pprof version ([#117](https://github.com/EmbarkStudios/pprof-rs/pull/117))
- add vdso to the blocklist in README.md ([#111](https://github.com/EmbarkStudios/pprof-rs/pull/111))
- Fix pthread_getname_np not available on musl ([#110](https://github.com/EmbarkStudios/pprof-rs/pull/110))
- Bump version to 0.7.0 ([#109](https://github.com/EmbarkStudios/pprof-rs/pull/109))
- add rust 1.56.0 to the ci matrix ([#108](https://github.com/EmbarkStudios/pprof-rs/pull/108))
- Update inferno requirement from 0.10 to 0.11 ([#107](https://github.com/EmbarkStudios/pprof-rs/pull/107))
- add msrv to the README.md ([#101](https://github.com/EmbarkStudios/pprof-rs/pull/101))
- Bump actions/checkout from 2 to 3 ([#105](https://github.com/EmbarkStudios/pprof-rs/pull/105))
- support rust-protobuf ([#106](https://github.com/EmbarkStudios/pprof-rs/pull/106))
- change to once_cell from lazy_static ([#103](https://github.com/EmbarkStudios/pprof-rs/pull/103))
- Update parking_lot requirement from 0.11 to 0.12 ([#99](https://github.com/EmbarkStudios/pprof-rs/pull/99))
- bump version to v0.6.2 ([#96](https://github.com/EmbarkStudios/pprof-rs/pull/96))
- add CHANGELOG ([#97](https://github.com/EmbarkStudios/pprof-rs/pull/97))
- *(derive)* add Clone directive to ProfilerGuardBuilder ([#95](https://github.com/EmbarkStudios/pprof-rs/pull/95))
- Add thread names and timing information to protobuf reports ([#90](https://github.com/EmbarkStudios/pprof-rs/pull/90))
- Fine tune the usage of `MaybeUninited` ([#89](https://github.com/EmbarkStudios/pprof-rs/pull/89))
- add allow(clippy::large_enum_variant) to Output ([#93](https://github.com/EmbarkStudios/pprof-rs/pull/93))
- migrate to rust 2021 ([#91](https://github.com/EmbarkStudios/pprof-rs/pull/91))
- bump version to v0.6.1 ([#87](https://github.com/EmbarkStudios/pprof-rs/pull/87))
- avoid deadlock by skipping sampling in libc, libgcc and pthread ([#85](https://github.com/EmbarkStudios/pprof-rs/pull/85))
- bump version to v0.6.0 ([#83](https://github.com/EmbarkStudios/pprof-rs/pull/83))
- bump deps and make clippy happy ([#82](https://github.com/EmbarkStudios/pprof-rs/pull/82))
- bump version to v0.5.0
- Bump prost* ([#73](https://github.com/EmbarkStudios/pprof-rs/pull/73))
- Bump actions-rs/cargo from 1 to 1.0.3 ([#63](https://github.com/EmbarkStudios/pprof-rs/pull/63))
- Bump actions-rs/toolchain from 1 to 1.0.7 ([#64](https://github.com/EmbarkStudios/pprof-rs/pull/64))
- bump version to v0.4.4
- add phantom data for criterion output ([#68](https://github.com/EmbarkStudios/pprof-rs/pull/68))
- modify document according to the current API ([#62](https://github.com/EmbarkStudios/pprof-rs/pull/62))
- bump version to v0.4.3
- Adjust the output paths `criterion::PProfProfiler` uses to support benchmark groups ([#59](https://github.com/EmbarkStudios/pprof-rs/pull/59))
- Update nix requirement from 0.19 to 0.20 ([#56](https://github.com/EmbarkStudios/pprof-rs/pull/56))
- bump version to v0.4.2
- Fix compilation error on arm architecture ([#55](https://github.com/EmbarkStudios/pprof-rs/pull/55))
- implement criterion Profiler ([#53](https://github.com/EmbarkStudios/pprof-rs/pull/53))
- bump version to v0.4.1
- allow passing custom flamegraph options ([#51](https://github.com/EmbarkStudios/pprof-rs/pull/51))
- bump version to v0.4.0
- bump version to v0.3.21
- give a reasonable hint for musl-libc based host ([#47](https://github.com/EmbarkStudios/pprof-rs/pull/47))
- Update rand requirement from 0.7.2 to 0.8.0 ([#46](https://github.com/EmbarkStudios/pprof-rs/pull/46))
- Update nix requirement from 0.17 to 0.19 ([#43](https://github.com/EmbarkStudios/pprof-rs/pull/43))
- Add dependabot to keep dependencies up to date ([#42](https://github.com/EmbarkStudios/pprof-rs/pull/42))
- bump version to v0.3.20
- split symbolic-demangle into multiple features
- bump version to 0.3.19
- ignore SIGPROF rather than default signal handler
- refactor frame.rs and parts of others ([#37](https://github.com/EmbarkStudios/pprof-rs/pull/37))
- Add license scan report and status ([#39](https://github.com/EmbarkStudios/pprof-rs/pull/39))
- bump to version 0.3.18
- Add Report::build_unresolved API ([#35](https://github.com/EmbarkStudios/pprof-rs/pull/35))
- Fix erroneous comment ([#34](https://github.com/EmbarkStudios/pprof-rs/pull/34))
- Remove extraneous `mut` ([#33](https://github.com/EmbarkStudios/pprof-rs/pull/33))
- bump to version 0.3.17
- Use criterion for benchmarking ([#30](https://github.com/EmbarkStudios/pprof-rs/pull/30))
- Replace spin with parking_lot ([#29](https://github.com/EmbarkStudios/pprof-rs/pull/29))
- Update README.md
- bump to version 0.3.16
- use symbolic_demangle
- bump to version 0.3.15
- filter out signal handler function
- filter out signal handler function
- bump to version 0.3.14
- get backtrace after getting lock
- remove lock in backtrace::backtrace
- bump version to 0.3.13
- only use thread name on linux and macos
- reset dependency version
- Miscellaneous tidying up
- bump version to v0.3.12
- stop timer before profiler stops
- Merge remote-tracking branch 'origin/master'
- turn collector into sum counter
- move collector data from stack to heap
- add benchmark
- Fix typo & add benchmark
- Add a image of pprof output
- update protobuf README.md and example
- upgrade version
- support protobuf
- merge with lonng's proto support
- update README.md and documentation
- update readme and documents
- insert badges into README.md
- update README.md
- add document of pprof
- add introduction to frame_post_processor in README.md
- update version
- smaller buffer length
- update README.md
- remove test on malloc
- update version
- update crate name
- update version
- add test for malloc
- use less stack space
- update README.md
- update version
- update version
- use pthread functions to get thread id and thread name
- make clippy happy!
- support frames post processor
- add thread_id and thread_name message in sampler and report
- update version
- update guard related codes
- update version
- modify README.md to use RwLock
- impl Send for Symbol
- resolve frame at report time
- update version
- unregister signal when start processing
- add some logs
- add guard support
- remove uneeded println!
- clear data after stop
- check for whether profiler is running
- remove uneeded use
- add repository in Cargo.toml
- add README.md and description
- ignore first two layers of profiler
- add flamegraph feature
- use symbol to seperate functions
- simple profiler
- Initial commit

## [0.13.0] - 2023-09-27

### Changed
- Upgrade `prost`, `prost-derive`, `prost-build` to 0.12 (#223)

## [0.12.1] - 2023-07-25

### Fixed
- Handle potentially unaligned frame pointer (#217)
- Fix the register field name according to libc (#218)

## [0.12.0] - 2023-07-03

### Added
- Support building `pprof-rs` for `android` target (#202)
- Support building `pprof-rs` for `freebsd` target (#213)

### Changed
- Upgrade `criterion` to 0.5 (#212)
- Bump the MSRV to 1.64.0 (#204)

### Fixed
- Hide `perf_signal_handler` frames on macOS (#207)

## [0.11.1] - 2023-02-21

### Added
- Support RISC-V architecture (#169)
- Support LoongArch64 architecture (#174)

### Fixed
- Use a globally shared pipe to validate memory to avoid FD leak (#198)

## [0.11.0] - 2022-11-03

### Changed
- Upgrade prost 0.11 (#166)
- Upgrade criterion from 0.3 to 0.4 (#163)

### Fixed
- Restart syscalls interuppted by SIGPROF when possible (#167)
- Only do per-frame-blocklist-check when frame-pointer is enabled (#172)

## [0.10.1] - 2022-08-29

### Changed
- Update `MAX_DEPTH` to 128 (#159)

### Fixed
- Fixed clippy warnnings and ignore prost mod (#160)

## [0.10.0] - 2022-06-27

### Changed
- Remove `backtrace-rs` feature, as the default choice when not specified (#130)

### Added
- Add `sample_timestamp` to Frames and UnresolvedFrames in order to have more fine-grained info on when the samples are collected (#133)
- 
### Fixed
- Export `UnresolvedReport` type to allow developers to get the unresolved report (#132)

## [0.9.1] - 2022-05-19

### Fixed
- Protect the error number in signal handler (#128)

## [0.9.0] - 2022-05-09

### Added
- Add `frame-pointer` feature to unwind the stack with frame pointer (#116)

### Changed
- The user has to specify one unwind implementation (`backtrace-rs` or `frame-pointer`) in the features (#116)

## [0.8.0] - 2022-04-20

### Changed
- Update prost from 0.9 to 0.10 (#113, #114, #115)

### Fixed
- Fix pthread_getname_np not available on musl (#110)

## [0.7.0] - 2022-03-08

### Added
- Add rust-protobuf support by adding protobuf-codec features (#106)

### Changed
- protobuf feature is renamed to prost-codec to align all other tikv projects (#106)

## [0.6.2] - 2021-12-24
### Added
- implement `Clone` for `ProfilerGuardBuilder` [@yangkeao](https://github.com/YangKeao)
- Add thread names and timing information to protobuf reports [@free](https://github.com/free)

## [0.6.1] - 2021-11-01
### Added
- `blocklist` to skip sampling in selected shared library [@yangkeao](https://github.com/YangKeao)

### Fixed
- Fix memory leak in collector of samples [@yangkeao](https://github.com/YangKeao)

## [0.6.0] - 2021-10-21
### Changed
- Bump prost* to v0.9.0 [@PsiACE](https://github.com/PsiACE)

### Security
- Bump nix to v0.23 [@PsiACE](https://github.com/PsiACE)

## [0.5.0] - 2021-10-21
### Changed
- Bump version of prost* [@PsiACE](https://github.com/PsiACE)

## [0.4.4] - 2021-07-13
### Fixed
- Fix the lifetime mark is not used by criterion output [@yangkeao](https://github.com/YangKeao)

## [0.4.3] - 2021-03-18
### Changed
- Change the output paths for `criterion::PProfProfiler` to support benchmark groups [@yangkeao](https://github.com/YangKeao)

### Security
- Bump nix to v0.20 [@yangkeao](https://github.com/YangKeao)

## [0.4.2] - 2021-02-20
### Added
- Implement criterion profiler [@yangkeao](https://github.com/YangKeao)

### Fixed
- Fix compilation error on arm architecture [@yangkeao](https://github.com/YangKeao)

## [0.4.1] - 2021-02-10
### Added
- Allow passing custom flamegraph options [@yangkeao](https://github.com/YangKeao)

## [0.4.0] - 2020-12-30
### Fix
- Fix flamegraph inline functions [@yangkeao](https://github.com/YangKeao)

## [0.3.21] - 2020-12-28
### Changed
- Bump version of prost* [@xhebox](https://github.com/xhebox)

### Security
- Bump rand to v0.8 @dependabot
- Bump nix to v0.19 @dependabot

## [0.3.20] - 2020-12-11
### Changed
- Split `symbolic-demangle` into multiple features [@yangkeao](https://github.com/YangKeao)

## [0.3.19] - 2020-12-11
### Fix
- Ignore SIGPROF signal after stop, rather than reset to the default handler [@yangkeao](https://github.com/YangKeao)

## [0.3.18] - 2020-08-07
### Added
- Add `Report::build_unresolved` [@umanwizard](https://github.com/umanwizard)

### Changed
- Change from `&mut self` to `&self` in `RpoertBuilder::build` [@umanwizard](https://github.com/umanwizard)

## [0.3.16] - 2020-02-25
### Added
- Support cpp demangle [@yangkeao](https://github.com/YangKeao)

## [0.3.15] - 2020-02-05
### Added
- Filter out signal handler functions [@yangkeao](https://github.com/YangKeao)

### Fixed
- Fix protobuf unit [@yangkeao](https://github.com/YangKeao)

## [0.3.14] - 2020-02-05
### Fixed
- Don't get lock inside `backtrace::Backtrace` [@yangkeao](https://github.com/YangKeao)

## [0.3.13] - 2020-01-31
### Added
- Export `prost::Message` [@yangkeao](https://github.com/YangKeao)

### Fixed
- Only use thread name on linux and macos [@yangkeao](https://github.com/YangKeao)
- Disable `#![feature(test)]` outside of tests [@kennytm](https://github.com/kennytm)

## [0.3.12] - 2019-11-27
### Fixed
- Stop timer before profiler stops [@yangkeao](https://github.com/YangKeao)

## [0.3.9] - 2019-11-08
### Added
- Support profobuf output [@lonng](https://github.com/lonng)

## [0.3.5] - 2019-11-04
### Changed
- Change crate name from `rsperftools` to `pprof-rs` [@yangkeao](https://github.com/YangKeao)

## [0.3.4] - 2019-11-04
### Changed
- Use less stack space [@yangkeao](https://github.com/YangKeao)

## [0.3.2] - 2019-11-01
### Fixed
- Seek to the start before reading file in `TempFdArray`[@yangkeao](https://github.com/YangKeao)

## [0.3.1] - 2019-11-01
### Added
- Support customized post processor for frames [@yangkeao](https://github.com/YangKeao)

### Fixed
- Fix deadlock inside the `std::thread::current().name()` [@yangkeao](https://github.com/YangKeao)

## [0.2.3] - 2019-10-31
### Fixed
- Avoid calling `malloc` inside the signal handler [@yangkeao](https://github.com/YangKeao)

## [0.1.4] - 2019-10-25
### Changed
- Implement `Send` for `Symbol` [@yangkeao](https://github.com/YangKeao)

## [0.1.3] - 2019-10-24
### Added
- Add log [@yangkeao](https://github.com/YangKeao)

### Fixed
- Stop signal handler after processing started [@yangkeao](https://github.com/YangKeao)

## [0.1.1] - 2019-10-22
### Added
- Check whether profiler is running when starting the profiler [@yangkeao](https://github.com/YangKeao)

## [0.1.0] - 2019-10-22
### Added
- Support profiling with signal handler [@yangkeao](https://github.com/YangKeao)
- Support generating flamegraph [@yangkeao](https://github.com/YangKeao)
