ballin-wookie
=============

1 contributor
22 lines (19 sloc)  0.403 kb RawBlameHistory  
buildscript {
    repositories {
        mavenCentral()
    }
    dependencies {
        classpath 'com.android.tools.build:gradle:0.9.2'
    }
}
apply plugin: 'android'

android {
    compileSdkVersion 'android-19'
    buildToolsVersion '19.1.0'

    buildTypes {
        release {
            runProguard false
            proguardFile getDefaultProguardFile('proguard-android.txt')
        }
    }
}
