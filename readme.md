# 项目结构

    |-- package-lock.json
    |-- package.json
    |-- adb
    |   |-- MyApplication
    |       |-- .gitignore
    |       |-- build.gradle.kts
    |       |-- gradle.properties
    |       |-- gradlew
    |       |-- gradlew.bat
    |       |-- local.properties
    |       |-- settings.gradle.kts
    |       |-- .gradle
    |       |   |-- config.properties
    |       |   |-- 8.11.1
    |       |   |   |-- gc.properties
    |       |   |   |-- checksums
    |       |   |   |   |-- checksums.lock
    |       |   |   |   |-- md5-checksums.bin
    |       |   |   |   |-- sha1-checksums.bin
    |       |   |   |-- executionHistory
    |       |   |   |   |-- executionHistory.lock
    |       |   |   |-- expanded
    |       |   |   |-- fileChanges
    |       |   |   |   |-- last-build.bin
    |       |   |   |-- fileHashes
    |       |   |   |   |-- fileHashes.bin
    |       |   |   |   |-- fileHashes.lock
    |       |   |   |-- vcsMetadata
    |       |   |-- buildOutputCleanup
    |       |   |   |-- buildOutputCleanup.lock
    |       |   |   |-- cache.properties
    |       |   |-- vcs-1
    |       |       |-- gc.properties
    |       |-- .idea
    |       |   |-- .gitignore
    |       |   |-- .name
    |       |   |-- AndroidProjectSystem.xml
    |       |   |-- appInsightsSettings.xml
    |       |   |-- compiler.xml
    |       |   |-- deploymentTargetSelector.xml
    |       |   |-- gradle.xml
    |       |   |-- kotlinc.xml
    |       |   |-- migrations.xml
    |       |   |-- misc.xml
    |       |   |-- runConfigurations.xml
    |       |   |-- workspace.xml
    |       |   |-- caches
    |       |   |-- inspectionProfiles
    |       |       |-- Project_Default.xml
    |       |-- app
    |       |   |-- .gitignore
    |       |   |-- build.gradle.kts
    |       |   |-- proguard-rules.pro
    |       |   |-- src
    |       |       |-- androidTest
    |       |       |   |-- java
    |       |       |       |-- com
    |       |       |           |-- example
    |       |       |               |-- myapplication
    |       |       |                   |-- ExampleInstrumentedTest.kt
    |       |       |-- main
    |       |       |   |-- AndroidManifest.xml
    |       |       |   |-- java
    |       |       |   |   |-- com
    |       |       |   |       |-- example
    |       |       |   |           |-- myapplication
    |       |       |   |               |-- MainActivity.kt
    |       |       |   |               |-- ui
    |       |       |   |                   |-- theme
    |       |       |   |                       |-- Color.kt
    |       |       |   |                       |-- Theme.kt
    |       |       |   |                       |-- Type.kt
    |       |       |   |-- res
    |       |       |       |-- drawable
    |       |       |       |   |-- ic_launcher_background.xml
    |       |       |       |   |-- ic_launcher_foreground.xml
    |       |       |       |-- mipmap-anydpi-v26
    |       |       |       |   |-- ic_launcher.xml
    |       |       |       |   |-- ic_launcher_round.xml
    |       |       |       |-- mipmap-hdpi
    |       |       |       |   |-- ic_launcher.webp
    |       |       |       |   |-- ic_launcher_round.webp
    |       |       |       |-- mipmap-mdpi
    |       |       |       |   |-- ic_launcher.webp
    |       |       |       |   |-- ic_launcher_round.webp
    |       |       |       |-- mipmap-xhdpi
    |       |       |       |   |-- ic_launcher.webp
    |       |       |       |   |-- ic_launcher_round.webp
    |       |       |       |-- mipmap-xxhdpi
    |       |       |       |   |-- ic_launcher.webp
    |       |       |       |   |-- ic_launcher_round.webp
    |       |       |       |-- mipmap-xxxhdpi
    |       |       |       |   |-- ic_launcher.webp
    |       |       |       |   |-- ic_launcher_round.webp
    |       |       |       |-- values
    |       |       |       |   |-- colors.xml
    |       |       |       |   |-- strings.xml
    |       |       |       |   |-- themes.xml
    |       |       |       |-- xml
    |       |       |           |-- backup_rules.xml
    |       |       |           |-- data_extraction_rules.xml
    |       |       |-- test
    |       |           |-- java
    |       |               |-- com
    |       |                   |-- example
    |       |                       |-- myapplication
    |       |                           |-- ExampleUnitTest.kt
    |       |-- gradle
    |           |-- libs.versions.toml
    |           |-- wrapper
    |               |-- gradle-wrapper.jar
    |               |-- gradle-wrapper.properties
    |-- script
        |-- .gitignore
        |-- package-lock.json
        |-- package.json
        |-- test.js

其中根目录下的两个主文件夹分别为script和adb,adb下的MyApplication文件夹为通过andriod studio创建的安卓虚拟机项目,script文件夹为运行Appium的js脚本







# 运行须知

#### 1:使用 `npm` 在全局范围内安装 Appium：

```
npm i -g appium
```

#### 2:运行命令

```
appium
```

#### 3:安装JDK和ANDROID SDK,配置JDK_HOME环境变量,ANDROID_HOME ANDROID_HOME_SDK环境变量

#### 4:安装驱动本身

由于 UiAutomator2 驱动是由核心 Appium 团队维护的，它有一个官方的驱动名称，你可以通过 [Appium 扩展 CLI](https://appium.io/docs/zh/latest/cli/extensions/) 轻松安装：

```
appium driver install uiautomator2
```

#### 5:在项目根文件夹运行命令:

```
appium
```

appium驱动被启动



#### 6:在ANDROID STUDIO中打开对应的虚拟机项目文件夹MyApplication,运行虚拟机



#### 7:在scirpt文件下运行命令:

```
node .\test.js
```

