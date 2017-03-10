gradlew.bat signingReport
上面的命令可以生成签名报告
可以在Project Struture（Ctrl+Shift+Alt+S）里的Signing选项卡里添加keystore
也可以直接在app里的build.gradle里手写添加。
android {
    signingConfigs {
        keystore {
            keyAlias 'android'
            keyPassword 'android'
            storeFile file('E:/AndroidWorkspace/Mobile/MobileApp/app/keystore/debug.keystore')
            storePassword 'android'
        }
    }
......
}
