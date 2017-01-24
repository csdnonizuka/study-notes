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
Android Studio 常用快捷键
Ctrl + O 重写方法的快捷键。
Content Assist名字换成了Class Name Completion。
快捷键是Ctrl+Alt+Space（空格键）。
●For循环的快速补全

For each loop：[variable name].for
For i loop／i从小到大：[variable name].fori
For i loop (reversed)／i从大到小：[variable name].forr
