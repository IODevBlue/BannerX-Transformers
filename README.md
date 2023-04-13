BannerX-Transformers
====================

[<img alt="GitHub release (latest by date)" src="https://img.shields.io/github/v/release/IODevBlue/BannerX-Transformers?label=Current Version&color=2CCCE4&style=for-the-badge&labelColor=0109B6">](https://github.com/IODevBlue/BannerX-Transformers/releases) <img alt="Repository Size" src="https://img.shields.io/github/repo-size/IODevBlue/BannerX-Transformers?color=2CCCE4&style=for-the-badge&labelColor=0109B6"> [<img alt="License" src="https://img.shields.io/github/license/IODevBlue/BannerX-Transformers?color=2CCCE4&style=for-the-badge&labelColor=0109B6">](http://www.apache.org/licenses/LICENSE-2.0) [<img alt="GitHub Repository stars" src="https://img.shields.io/github/stars/IODevBlue/BannerX-Transformers?color=2CCCE4&style=for-the-badge&labelColor=0109B6">](https://github.com/IODevBlue/BannerX-Transformers/stargazers)
<img alt="GitHub watchers" src="https://img.shields.io/github/watchers/IODevBlue/BannerX-Transformers?label=Repository Watchers&color=2CCCE4&style=for-the-badge&labelColor=0109B6"> [<img alt="Gradle version" src="https://img.shields.io/static/v1?label=Gradle version&message=7.5.1&color=2CCCE4&style=for-the-badge&labelColor=0109B6">](https://docs.gradle.org/7.5.1/release-notes) [<img alt="Kotlin version" src="https://img.shields.io/static/v1?label=Kotlin version&message=1.7.10&color=2CCCE4&style=for-the-badge&labelColor=0109B6">](https://KOTLINlang.org/docs/whatsnew1720)

Table of content
----------------
- [Documentations](https://github.com/IODevBlue/BannerX-Transformers/tree/main#documentations)
- [Uses](https://github.com/IODevBlue/BannerX-Transformerstree/main#uses)
- [Installation](https://github.com/IODevBlue/BannerX-Transformerstree/main#installation)
- [Contributions](https://github.com/IODevBlue/BannerX-Transformerstree/main#contributions)
- [Change log](https://github.com/IODevBlue/BannerX-Transformerstree/main#change-log)
- [License](https://github.com/IODevBlue/BannerX-Transformerstree/main#license)

Documentations
--------------
Documentations are available online in [Javadoc](https://raw.githack.com/IODevBlue/BannerX-Transformers/main/_docs/javadoc/index.html) and [KDoc](https://raw.githack.com/IODevBlue/BannerX-Transformers/main/_docs/html/index.html).

Uses
----
BannerX-Transformers is only used as an extension of the [BannerX](https://github.com/IODevBlue/BannerX) library.

<details>
  <summary>AccordionBannerTransformer</summary>
  <p align="center"><img src="https://github.com/IODevBlue/sample-previews/blob/main/api/android/bannerx-transformers/accordion.gif" alt="AccordionBannerTransformer"></p>
</details>

<details>
  <summary>AlphaBannerTransformer</summary>
  <p align="center"><img src="https://github.com/IODevBlue/sample-previews/blob/main/api/android/bannerx-transformers/alpha.gif" alt="AlphaBannerTransformer"></p>
</details>

<details>
  <summary>CartwheelBannerTransformer</summary>
  <p align="center"><img src="https://github.com/IODevBlue/sample-previews/blob/main/api/android/bannerx-transformers/cartwheel.gif" alt="CartwheelBannerTransformer"></p>
</details>

<details>
  <summary>CenterScaleBannerTransformer</summary>
  <p align="center"><img src="https://github.com/IODevBlue/sample-previews/blob/main/api/android/bannerx-transformers/centerscale.gif" alt="CenterScaleBannerTransformer"></p>
</details>

<details>
  <summary>DescentBannerTransformer</summary>
  <p align="center"><img src="https://github.com/IODevBlue/sample-previews/blob/main/api/android/bannerx-transformers/descent.gif" alt="DescentBannerTransformer"></p>
</details>

<details>
  <summary>FlipBannerTransformer</summary>
  <p align="center"><img src="https://github.com/IODevBlue/sample-previews/blob/main/api/android/bannerx-transformers/flip.gif" alt="FlipBannerTransformer"></p>
</details>

<details>
  <summary>OverlayBannerTransformer</summary>
  <p align="center"><img src="https://github.com/IODevBlue/sample-previews/blob/main/api/android/bannerx-transformers/overlay.gif" alt="OverlayBannerTransformer"></p>
</details>

<details>
  <summary>PunchyBannerTransformer</summary>
  <p align="center"><img src="https://github.com/IODevBlue/sample-previews/blob/main/api/android/bannerx-transformers/punchy.gif" alt="PunchyBannerTransformer"></p>
</details>

<details>
  <summary>ScaleBannerTransformer</summary>
  <p align="center"><img src="https://github.com/IODevBlue/sample-previews/blob/main/api/android/bannerx-transformers/scale.gif" alt="ScaleBannerTransformer"></p>
</details>

<details>
  <summary>SidedStackBannerTransformer</summary>
  <p align="center"><img src="https://github.com/IODevBlue/sample-previews/blob/main/api/android/bannerx-transformers/sidedstack.gif" alt="SidedStackBannerTransformer"></p>
</details>


Installation
------------
1. Grab a JAR artifact from the Maven Central Repository:
```GROOVY
implementation 'io.github.iodevblue:bannerx-transformers:1.0.0'
```
- On Apache Maven
```XML
<dependency>
  <groudId> io.github.iodevblue </groudId>
  <artifactId> bannerx-transformers </artifactId>
  <version> 1.0.0 </version>
</dependency>
```
If it is a snapshot version, add the snapshot Maven Nexus OSS repository:
```GROOVY
maven {   
  url 'https://s01.oss.sonatype.org/content/repositories/snapshots/'
}
```
Then retrieve a copy:
```GROOVY
implementation 'io.github.iodevblue:bannerx-transformers:1.0.0-SNAPSHOT'
```

2. Grab a JAR artifact from the [release](https://github.com/IODevBlue/BannerX-Transformers/releases) section.
- Place it in `libs` folder in your project module and install in your project.
```GROOVY
implementation fileTree(dir:' libs', include:'*jar')
```

Contributions
-------------
Contributors are welcome!

**NOTE:** This repository is split into two branches:
- [main](https://github.com/IODevBlue/BannerX-Transformers/tree/main) branch
- [development](https://github.com/IODevBlue/BannerX-Transformers/tree/development) branch
All developing implementations and proposed changes are pushed to the [development](https://github.com/IODevBlue/BannerX-Transformers/tree/development) branch and finalized updates are pushed to the [main](https://github.com/IODevBlue/BannerX-Transformers/tree/main) branch.

To note if current developments are being made, there would be more commits in the [development](https://github.com/IODevBlue/BannerX-Transformers/tree/development) branch than in the [main](https://github.com/IODevBlue/BannerX-Transformers/tree/main) branch.

A [BannerX](https://github.com/IODevBlue/BannerX) transformer is simply a [ViewPager2.PageTransformer](https://developer.android.com/reference/kotlin/androidx/viewpager2/widget/ViewPager2.PageTransformer) that implements the `Parcelable` interface.

Check the [Contributing](https://github.com/IODevBlue/BannerX-Transformers/blob/development/CONTRIBUTING.md) for more information.


Changelog
---------
* **1.0.0**
    * Initial release

More version history can be gotten from the [Change log](https://github.com/IODevBlue/BannerX-Transformers/blob/main/CHANGELOG.md) file.


License
=======
```
    Copyright 2023 IO DevBlue

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
```