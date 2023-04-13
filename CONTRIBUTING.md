Contributing
============

<img alt="GitHub forks" src="https://img.shields.io/github/forks/IODevBlue/BannerX-Transformers?label=Forks&color=2CCCE4&style=for-the-badge&labelColor=0109B6"> <img alt="Number of issues" src="https://img.shields.io/github/issues-raw/IODevBlue/BannerX-Transformers?color=2CCCE4&style=for-the-badge&labelColor=0109B6"> <img alt="Closed issues" src="https://img.shields.io/github/issues-closed-raw/IODevBlue/BannerX-Transformers?color=2CCCE4&style=for-the-badge&labelColor=0109B6">

<img alt="Number of pull requests" src="https://img.shields.io/github/issues-pr-raw/IODevBlue/BannerX-Transformers?color=2CCCE4&style=for-the-badge&labelColor=0109B6"> <img alt="Closed pull requests" src="https://img.shields.io/github/issues-pr-closed-raw/IODevBlue/BannerX-Transformers?color=2CCCE4&style=for-the-badge&labelColor=0109B6">

<img alt="GitHub contributors" src="https://img.shields.io/github/contributors/IODevBlue/BannerX-Transformers?color=2CCCE4&style=for-the-badge&labelColor=0109B6">

<img alt="Last commit for development" src="https://img.shields.io/github/last-commit/IODevBlue/BannerX-Transformers/development?color=2CCCE4&style=for-the-badge&labelColor=0109B6">

Current tasks to be completed
-----------------------------
No tasks available!

- Have a new feature in mind?
- Want to make changes and improvements to documentations and code?
- Noticed an error?
- Found a bug?

Contributions are welcome and encouraged!!

Make a [fork](https://github.com/IODevBlue/BannerX-Transformers/fork) of the repository and send a pull request.

Discussions about your code, logical decisions and proposed changes would be made before pushing to the [main](https://github.com/IODevBlue/BannerX-Transformers/tree/main) repository branch.

To get started with contributions, get the `BannerX` library artifact from the Maven Central Repository:
```GROOVY
implementation 'io.github.iodevblue:bannerx:1.0.0'
```
- On Apache Maven
```XML
<dependency>
  <groudId> io.github.iodevblue </groudId>
  <artifactId> bannerx </artifactId>
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
implementation 'io.github.iodevblue:bannerx:1.0.0-SNAPSHOT'
```

**NOTE:** All `BannerX` transformers **MUST** follow the naming pattern: (name)BannerTransformer.
For example: GithubBannerTransformer, CommitBannerTransformer, CodeBannerTransformer etc.

Every `BannerX` transformer extends the `BannerXTransformer` abstract class and **must** implement the `Parcelable` interface. 
However, all transformer classes currently use the `@Parcelize` Kotlin annotation to automatically generate `Parcelable` methods, manual implementations of the `Parcelable` interface methods work fine as well.

If your transformer exposes variables used for transformation, you would have to persist those variables using a static `Parceler` implementation:
```kotlin
var alphaSeed: Float = 0.5F 
    set(value) { //Setter exposed to the programmer
        if(value in 0.0F..1.0F) { 
            field = value 
        }
    }

private companion object: Parceler<AlphaBannerTransformer> {
    override fun create(parcel: Parcel): AlphaBannerTransformer {
        return AlphaBannerTransformer().apply {
            alphaSeed = parcel.readFloat() //Read value from Parcel
        }
    }

    override fun AlphaBannerTransformer.write(parcel: Parcel, flags: Int) {
        parcel.writeFloat(alphaSeed) //Write value into Parcel
    }

}
```
Refer to the [AlphaBannerTransformer](https://github.com/IODevBlue/BannerX/tree/main/bannerx-transformers/src/main/kotlin/com/blueiobase/api/android/bannerx/transformers/AlphaBannerTransformer.kt) for more details.


Concerning Issues
-----------------
- Before creating an issue, please verify if a pre-existing and similar issue already exists. 
- If an issue is closed and problem persists, you can reopen that same issue or create an entirely new issue.
- Persistent bugs can be better illustrated using a unit/integrated test, demo project, JPG/JPEG file, GIF animation, stack traces and logs.

**NOTE:** When posting code blocks, logs or stack traces etc, please use Github flavoured markdown syntax to improve readability.

For Kotlin code blocks, KDoc comments with KDoc syntax are preferable.

Concerning Code Style
---------------------
Consistent indentation plays an important role in readability and maintainability of code. 
The indentation currently used in this project is as follows:
```KOTLIN
fun correctIndent() {
	doSomethingHere {
		val x = "some string var"
	}
}
```
Wrong indentation:
```KOTLIN
fun inCorrectIndent() 
{
	doSomethingHere 
	{
		val x = "some string var"
	}
}
```
Please follow the correct indentation style.