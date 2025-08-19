# Change Log for Amazon Corretto 25

The following sections describe the changes for each release of Amazon Corretto 25.
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