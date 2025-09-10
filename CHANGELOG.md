# Change Log for Amazon Corretto 25

The following sections describe the changes for each release of Amazon Corretto 25.
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
+ macos 13.0 and later, x86_64
+ macos 13.0 and later, aarch64
 
 
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
+ macos 13.0 and later, x86_64
+ macos 13.0 and later, aarch64
 
 
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
+ macos 13.0 and later, x86_64
+ macos 13.0 and later, aarch64
 
 
**1.** This is the platform targeted by the build. See [Using Amazon Corretto](https://aws.amazon.com/corretto/faqs/#Using_Amazon_Corretto)
in the Amazon Corretto FAQ for supported platforms
 
The following issues are addressed in 25.0.0.34.1:
 
| Issue Name       | Platform | Description                                | Link                                                               |
|------------------|----------|--------------------------------------------|--------------------------------------------------------------------|
| Import jdk-25+34 | All      | Updates Corretto baseline to OpenJDK 25+34 | [jdk-25+34](https://github.com/openjdk/jdk/releases/tag/jdk-25+34) |