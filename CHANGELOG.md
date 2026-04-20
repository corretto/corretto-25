# Change Log for Amazon Corretto 25

The following sections describe the changes for each release of Amazon Corretto 25.

## Corretto version: 25.0.3.9.1
Release Date: April 21, 2026
 
**Target Platforms**
 
+ RPM-based Linux using glibc 2.17 or later, x86_64
+ Debian-based Linux using glibc 2.17 or later, x86_64
+ RPM-based Linux using glibc 2.17 or later, aarch64
+ Debian-based Linux using glibc 2.17 or later, aarch64
+ Alpine-based Linux, x86_64
+ Alpine-based Linux, aarch64
+ Windows 11 or later, x86_64
+ macOS 14.0 and later, x86_64
+ macOS 14.0 and later, aarch64
 
The following issues above are addressed in 25.0.3.9.1

| Issue Name | Platform | Description | Link |
|------------|----------|-------------|------|
| Import jdk-25.0.3+9 | All | Updates Corretto baseline to OpenJDK 25.0.3+9 | [jdk-25.0.3+9](https://github.com/openjdk/jdk25u/releases/tag/jdk-25.0.3+9) |
| JDK-8381670 | All | Revert the changes to GZIPInputStream related to InputStream… | [#56](https://github.com/corretto/corretto-25/pull/56) |
| JDK-8373120 | All | Virtual thread stuck in BLOCKED state | [#53](https://github.com/corretto/corretto-25/pull/53) |
| JDK-8376104 | All | C2 crashes in PhiNode::Ideal(PhaseGVN*, bool) accessing NULL pointer | [#51](https://github.com/corretto/corretto-25/pull/51) |
| JDK-8361699 | All | C2: assert(can_reduce_phi(n->as_Phi())) failed: Sanity: previous reducible Phi is no longer reducible before SUT | [#50](https://github.com/corretto/corretto-25/pull/50) |
| JDK-8339526 | All | C2: store incorrectly removed for clone() transformed to series of loads/stores | [#49](https://github.com/corretto/corretto-25/pull/49) |
| JDK-8377932 | All | AOT cache is not rejected when JAR file has changed | [#48](https://github.com/corretto/corretto-25/pull/48) |
| JDK-8370939 | All | C2: SIGSEGV in SafePointNode::verify_input when processing MH call from Compile::process_late_inline_calls_no_inline() | [#47](https://github.com/corretto/corretto-25/pull/47) |

The following CVEs are addressed in 25.0.3.9.1

| CVE | CVSS | Component |
|-----|------|-----------|
| CVE-2026-22016 | 7.5 | xml/jaxp |
| CVE-2026-34282 | 7.5 | core-libs/java.net |
| CVE-2026-22021 | 5.3 | security-libs/java.security |
| CVE-2026-22013 | 5.3 | security-libs/org.ietf.jgss |
| CVE-2026-23865 | 5.3 | client-libs/2d |
| CVE-2026-22008 | 3.7 | core-libs/java.lang |
| CVE-2026-22020 | 7.1 | hotspot/compiler |
| CVE-2026-22018 | 3.7 | core-libs/java.util |
| CVE-2026-22007 | 2.9 | security-libs/java.security |
| CVE-2026-34268 | 2.9 | security-libs/java.security |

## Corretto version: 25.0.2.10.1
Release Date: January 20, 2026

**Target Platforms**

+ RPM-based Linux using glibc 2.17 or later, x86_64
+ Debian-based Linux using glibc 2.17 or later, x86_64
+ RPM-based Linux using glibc 2.17 or later, aarch64
+ Debian-based Linux using glibc 2.17 or later, aarch64
+ Alpine-based Linux, x86_64
+ Alpine-based Linux, aarch64
+ Windows 10 or later, x86_64
+ macOS 14.0 and later, x86_64
+ macOS 14.0 and later, aarch64

The following issues above are addressed in 25.0.2.10.1

| Issue Name | Platform | Description | Link |
|------------|----------|-------------|------|
| Import jdk-25.0.2+10 | All | Updates Corretto baseline to OpenJDK 25.0.2+10 | [jdk-25.0.2+10](https://github.com/openjdk/jdk25u/releases/tag/jdk-25.0.2+10) |
| JDK-8373630 | aarch64 | r18_tls should not be modified on Windows AArch64 | [#38](https://github.com/corretto/corretto-25/pull/38) |
| JDK-8371368 | aarch64 | SIGSEGV in JfrVframeStream::next_vframe() on arm64 | [#37](https://github.com/corretto/corretto-25/pull/37) |
| JDK-8370405 | All | C2: mismatched store from MergeStores wrongly scalarized in allocation elimination | [#36](https://github.com/corretto/corretto-25/pull/36) |
| JDK-8361492 | All | [IR Framework] Has too restrictive regex for load and store | [#35](https://github.com/corretto/corretto-25/pull/35) |
| JDK-8369050 | All | DecimalFormat Rounding Errors for Fractional Ties Near Zero | [#34](https://github.com/corretto/corretto-25/pull/34) |
| JDK-8368182 | All | AOT cache creation fails with class defined by JNI | [#33](https://github.com/corretto/corretto-25/pull/33) |
| JDK-8370887 | All | DelayScheduler.replace method may break the 4-ary heap in certain scenarios | [#32](https://github.com/corretto/corretto-25/pull/32) |
| Revert Update Corretto version | All | Revert "Update Corretto version to match upstream: 25.0.3.0.1" | [#31](https://github.com/corretto/corretto-25/pull/31) |
| JDK-8371864 | All | GaloisCounterMode.implGCMCrypt0 AVX512/AVX2 intrinsics stubs cause AES-GCM encryption failure for certain payload sizes | [#30](https://github.com/corretto/corretto-25/pull/30) |
| Add additional build targets option for Mac | macOS | Add additional build targets option for Mac | [#29](https://github.com/corretto/corretto-25/pull/29) |
| JDK-8359472 | All | JVM crashes when attaching a dynamic agent before JVMTI_PHASE_LIVE | [#340](https://github.com/openjdk/jdk25u/pull/340) |
| JDK-8370242 | All | JFR: Clear event reference eagerly when using EventStream | [#372](https://github.com/openjdk/jdk25u/pull/372) |
| JDK-8372534 | All | Update Libpng to 1.6.51 | [JDK-8372534](https://bugs.openjdk.org/browse/JDK-8372534) |

The following CVEs are addressed in 25.0.2.10.1

| CVE | CVSS | Component |
|-----|------|-----------|
| CVE-2026-21945 | 7.5 | security-libs/java.security |
| CVE-2026-21932 | 7.4 | client-libs/java.awt |
| CVE-2026-21933 | 6.1 | core-libs/java.net |
| CVE-2026-21925 | 4.8 | core-libs/java.rmi |

## Corretto version: 25.0.1.9.1
Release Date: November 3, 2025

**Target Platforms <sup>1</sup>**

+ RPM-based Linux using glibc 2.17 or later, x86_64
+ Debian-based Linux using glibc 2.17 or later, x86_64
+ RPM-based Linux using glibc 2.17 or later, aarch64
+ Debian-based Linux using glibc 2.17 or later, aarch64
+ Alpine-based Linux, x86_64
+ Alpine-based Linux, aarch64


**1.** This is the platform targeted by the build. See [Using Amazon Corretto](https://aws.amazon.com/corretto/faqs/#Using_Amazon_Corretto)
in the Amazon Corretto FAQ for supported platforms

The following issues are addressed in 25.0.1.9.1:

| Issue Name       | Platform | Description                                | Link                                                               |
|------------------|----------|--------------------------------------------|--------------------------------------------------------------------|
| JDK-8370572 | Linux | 8370572: cgroup v1 hierarchical memory limit is not honored after JDK-8322420 | [JDK-8370572](https://bugs.openjdk.org/browse/JDK-8370572) |
| JDK-8365153 | All Aarch64 | AArch64: Set JVM flags for Neoverse N3 and V3 cores | [JDK-8365153](https://bugs.openjdk.org/browse/JDK-8365153) |

## Corretto version: 25.0.1.8.1
Release Date: October 21, 2025

**Target Platforms <sup>1</sup>**

+ RPM-based Linux using glibc 2.17 or later, x86_64
+ Debian-based Linux using glibc 2.17 or later, x86_64
+ RPM-based Linux using glibc 2.17 or later, aarch64
+ Debian-based Linux using glibc 2.17 or later, aarch64
+ Alpine-based Linux, x86_64
+ Alpine-based Linux, aarch64
+ Windows 10 or later, x86_64
+ macOS 14.0 and later, x86_64
+ macOS 14.0 and later, aarch64


**1.** This is the platform targeted by the build. See [Using Amazon Corretto](https://aws.amazon.com/corretto/faqs/#Using_Amazon_Corretto)
in the Amazon Corretto FAQ for supported platforms

The following issues above are addressed in 25.0.1.8.1:

| Issue Name | Platform | Description | Link |
|------------|----------|-------------|------|
| Import jdk-25.0.1+8 | All | Updates Corretto baseline to OpenJDK 25.0.1+8 | [jdk-25.0.1+8](https://github.com/openjdk/jdk25u/releases/tag/jdk-25.0.1+8)
| JDK-8367333 | All | C2: Vector math operation intrinsification failure | [JDK-8367333](https://bugs.openjdk.org/browse/JDK-8367333) |
| JDK-8362282 | All | runtime/logging/StressAsyncUL.java failed with exitValue = 134 | [JDK-8362282](https://bugs.openjdk.org/browse/JDK-8362282) |
| JDK-8365726 | All | Test crashed with assert in C1 thread: Possible safepoint reached by thread that does not allow it | [JDK-8365726](https://bugs.openjdk.org/browse/JDK-8365726) |
| JDK-8366948 | All | AOT cache creation crashes when iterating training data | [JDK-8366948](https://bugs.openjdk.org/browse/JDK-8366948) |
| JDK-8368698 | All | runtime/cds/appcds/aotCache/OldClassSupport.java assert(can_add()) failed: Cannot add TrainingData objects | [JDK-8368698](https://bugs.openjdk.org/browse/JDK-8368698) |
| JDK-8367689 | All | Revert removal of several compilation-related vmStructs fields | [JDK-8367689](https://bugs.openjdk.org/browse/JDK-8367689) |
| JDK-8364184 | All | [REDO] AArch64: [VectorAPI] sve vector math operations are not supported after JDK-8353217 | [JDK-8364184](https://bugs.openjdk.org/browse/JDK-8364184) |
| JDK-8366434 | All | THP not working properly with G1 after JDK-8345655 | [JDK-8366434](https://bugs.openjdk.org/browse/JDK-8366434) |
| JDK-8366980 | All | TestTransparentHugePagesHeap.java fails when run with -UseCompressedOops | [JDK-8366980](https://bugs.openjdk.org/browse/JDK-8366980) |
| JDK-8358535 | All | Changes in ClassValue (JDK-8351996) caused a 1-9% regression in Renaissance-PageRank | [JDK-8358535](https://bugs.openjdk.org/browse/JDK-8358535) |
| JDK-8357959 | All | (bf) ByteBuffer.allocateDirect initialization can result in large TTSP spikes | [JDK-8357959](https://bugs.openjdk.org/browse/JDK-8357959) |
| JDK-8368071 | All | Compilation throughput regressed 2X-8X after JDK-8355003 | [JDK-8368071](https://bugs.openjdk.org/browse/JDK-8368071) |
| JDK-8368152 | All | Shenandoah: Incorrect behavior at end of degenerated cycle | [JDK-8368152](https://bugs.openjdk.org/browse/JDK-8368152) |
| JDK-8357396 | All | 8357396: Refactor nmethod::make_not_entrant to use Enum instead of "const char*" | [JDK-8357396](https://bugs.openjdk.org/browse/JDK-8357396) |
| JDK-8277444 | All | 8277444: Data race between JvmtiClassFileReconstituter::copy_bytecodes and class linking | [JDK-8277444](https://bugs.openjdk.org/browse/JDK-8277444) |
| JDK-8362193 | aarch64 | 8362193: Re-work MacOS/AArch64 SpinPause to handle SB | [JDK-8362193](https://bugs.openjdk.org/browse/JDK-8362193) |
| JDK-8359435 | aarch64 | 8359435: AArch64: add support for SB instruction to MacroAssembler::spin_wait | [JDK-8359435](https://bugs.openjdk.org/browse/JDK-8359435) |
| Bundling async profiler | macOS, RPM-based Linux, Debian-based Linux, Alpine Linux | Binaries for the [async-profiler](https://github.com/async-profiler/async-profiler) are included in official builds for supported platforms | [#19](https://github.com/corretto/corretto-25/pull/19) |
| Expose reason for marking nmethod non-entrant to JVMCI client | All | Backport of "Expose reason for marking nmethod non-entrant to JVMCI client". Relates to JDK-8359064 and JDK-8360049 | [#18](https://github.com/corretto/corretto-25/pull/18) |
| Don't set OnSpinWaitInst to SB if VM_Version does not support it | All | Don't set OnSpinWaitInst to SB if VM_Version does not support it | [#17](https://github.com/corretto/corretto-25/pull/17) |
| Set OnSpinWaitInst to SB for Graviton 4 | aarch64 | Sets the default value for the OnSpinWaitInst flag to "sb" if the CPU model matches 0xd4f (Neoverse-V2); otherwise, it remains "isb" | [#11](https://github.com/corretto/corretto-25/pull/11) |

The following CVEs are addressed in 25.0.1.8.1:

| CVE | CVSS | Component |
|-----|------|-----------|
| CVE-2025-53057 | 5.9 | security-libs/java.security |
| CVE-2025-53066 | 4.8 | xml/jaxp |
| CVE-2025-61748 | 3.7 | core-libs |

## Corretto version: 25.0.0.36.2
Release Date: September 16, 2025

**Target Platforms <sup>1</sup>**

+ RPM-based Linux using glibc 2.17 or later, x86_64
+ Debian-based Linux using glibc 2.17 or later, x86_64
+ RPM-based Linux using glibc 2.17 or later, aarch64
+ Debian-based Linux using glibc 2.17 or later, aarch64
+ Alpine-based Linux, x86_64
+ Alpine-based Linux, aarch64
+ Windows 10 or later, x86_64
+ macOS 13.0 and later, x86_64
+ macOS 13.0 and later, aarch64


**1.** This is the platform targeted by the build. See [Using Amazon Corretto](https://aws.amazon.com/corretto/faqs/#Using_Amazon_Corretto)
in the Amazon Corretto FAQ for supported platforms

The following issues are addressed in 25.0.0.36.2:

| Issue Name       | Platform | Description                                | Link                                                               |
|------------------|----------|--------------------------------------------|--------------------------------------------------------------------|
| JDK-8364159 | All | Shenandoah assertions after JDK-8361712 | [JDK-8364159](https://bugs.openjdk.org/browse/JDK-8364159) |
| JDK-8365571 | All | GenShen: PLAB promotions may remain disabled for evacuation threads | [JDK-8365571](https://bugs.openjdk.org/browse/JDK-8365571) |
| JDK-8364183 | All | Shenandoah: Improve commit/uncommit handling | [JDK-8364183](https://bugs.openjdk.org/browse/JDK-8364183) |
| JDK-8361712 | All | Improve ShenandoahAsserts printing | [JDK-8361712](https://bugs.openjdk.org/browse/JDK-8361712) |
| JDK-8357818 | All | Shenandoah doesn't use shared API for printing heap before/after GC | [JDK-8357818](https://bugs.openjdk.org/browse/JDK-8357818) |
| JDK-8361948 | All | Shenandoah: region free capacity unit mismatch | [JDK-8361948](https://bugs.openjdk.org/browse/JDK-8361948) |
| JDK-8361342 | All | Shenandoah: Evacuation may assert on invalid mirror object after JDK-8340297 | [JDK-8361342](https://bugs.openjdk.org/browse/JDK-8361342) |
| JDK-8361363 | All | ShenandoahAsserts::print_obj() does not work for forwarded objects and UseCompactObjectHeaders | [JDK-8361363](https://bugs.openjdk.org/browse/JDK-8361363) |
| JDK-8359868 | All | Shenandoah: Free threshold heuristic does not use SoftMaxHeapSize | [JDK-8359868](https://bugs.openjdk.org/browse/JDK-8359868) |
| JDK-8358529 | All | GenShen: Heuristics do not respond to changes in SoftMaxHeapSize | [JDK-8358529](https://bugs.openjdk.org/browse/JDK-8358529) |

## Corretto version: 25.0.0.36.1
Release Date: August 21, 2025

**Target Platforms <sup>1</sup>**

+ RPM-based Linux using glibc 2.17 or later, x86_64
+ Debian-based Linux using glibc 2.17 or later, x86_64
+ RPM-based Linux using glibc 2.17 or later, aarch64
+ Debian-based Linux using glibc 2.17 or later, aarch64
+ Alpine-based Linux, x86_64
+ Alpine-based Linux, aarch64
+ Windows 10 or later, x86_64
+ macOS 13.0 and later, x86_64
+ macOS 13.0 and later, aarch64


**1.** This is the platform targeted by the build. See [Using Amazon Corretto](https://aws.amazon.com/corretto/faqs/#Using_Amazon_Corretto)
in the Amazon Corretto FAQ for supported platforms

The following issues are addressed in 25.0.0.36.1:

| Issue Name       | Platform | Description                                | Link                                                               |
|------------------|----------|--------------------------------------------|--------------------------------------------------------------------|
| Import jdk-25+36 | All      | Updates Corretto baseline to OpenJDK 25+36 | [jdk-25+36](https://github.com/openjdk/jdk/releases/tag/jdk-25+36) |
| Turn off interface/abstract class optimization | All | Turn off interface/abstract class optimization for non-class metaspace allocation | [PR-5](https://github.com/corretto/corretto-25/pull/5) |
| JDK-8343218 | All | Add option to disable allocating interface and abstract classes in non-class metaspace | [PR-3](https://github.com/corretto/corretto-25/pull/3) |
| Backport: Upgrade to Gradle 8.14.3 | All | Upgrade to Gradle 8.14.3 | [PR-6](https://github.com/corretto/corretto-25/pull/6) |

## Corretto version: 25.0.0.34.1
Release Date: August 7, 2025

**Target Platforms <sup>1</sup>**

+ RPM-based Linux using glibc 2.17 or later, x86_64
+ Debian-based Linux using glibc 2.17 or later, x86_64
+ RPM-based Linux using glibc 2.17 or later, aarch64
+ Debian-based Linux using glibc 2.17 or later, aarch64
+ Alpine-based Linux, x86_64
+ Alpine-based Linux, aarch64
+ Windows 10 or later, x86_64
+ macOS 13.0 and later, x86_64
+ macOS 13.0 and later, aarch64


**1.** This is the platform targeted by the build. See [Using Amazon Corretto](https://aws.amazon.com/corretto/faqs/#Using_Amazon_Corretto)
in the Amazon Corretto FAQ for supported platforms

The following issues are addressed in 25.0.0.34.1:

| Issue Name       | Platform | Description                                | Link                                                               |
|------------------|----------|--------------------------------------------|--------------------------------------------------------------------|
| Import jdk-25+34 | All      | Updates Corretto baseline to OpenJDK 25+34 | [jdk-25+34](https://github.com/openjdk/jdk/releases/tag/jdk-25+34) |
