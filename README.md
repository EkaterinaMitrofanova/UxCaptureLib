# UxCaptureLib

Add it in your root build.gradle:

    dependencies {
       ...
       classpath "io.realm:realm-gradle-plugin:5.0.0"
    }

    allprojects {
      repositories {
        ...
        maven { url 'https://jitpack.io' }
      }
    }
    
Add the dependency:

    dependencies {
      implementation 'com.github.EkaterinaMitrofanova:UxCaptureLib:1.0'
      implementation 'com.android.support:recyclerview-v7:26.1.0'
      implementation 'com.squareup.retrofit2:converter-gson:2.3.0'
      implementation 'com.squareup.retrofit2:retrofit:2.3.0'
      implementation 'com.squareup.retrofit2:adapter-rxjava2:2.3.0'
      implementation 'io.reactivex.rxjava2:rxjava:2.1.14-RC1'
      implementation 'io.reactivex.rxjava2:rxandroid:2.0.2'
    }
    
Add in build.gradle:

    apply plugin: 'realm-android'
    
    android {
      ...
      compileOptions {
          targetCompatibility 1.8
          sourceCompatibility 1.8
      }
    }
    
    realm {
      syncEnabled = true;
    }
