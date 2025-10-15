# Change Log for Amazon Corretto 25

The following sections describe the changes for each release of Amazon Corretto 25.

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
+ macOS 13.0 and later, x86_64
+ macOS 13.0 and later, aarch64


**1.** This is the platform targeted by the build. See [Using Amazon Corretto](https://aws.amazon.com/corretto/faqs/#Using_Amazon_Corretto)
in the Amazon Corretto FAQ for supported platforms

The following issues above are addressed in 25.0.1.8.1:

| Issue Name | Platform | Description | Link |
|------------|----------|-------------|------|
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
| Bundling async profiler | Alpine, macOS, RPM-based Linux, Debian-based Linux  | Binaries for the [async-profiler](https://github.com/async-profiler/async-profiler/tags) are included in official builds for supported platforms | [#19](https://github.com/corretto/corretto-25/pull/19) |

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
