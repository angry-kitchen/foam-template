# aphone升级 AndroidX 步骤：

1. 在gradle.properties 添加

 使用androidx

```
android.useAndroidX=true
```

将第三方库迁移到 androidx

```
android.enableJetifier=true
```

2. 点击菜单项中的Refactor中的Migratet to AndroidX

3. File->Invalidate Caches / restart

4. 修改 bsextend 里FixedFragmentStatePagerAdapter 的包名 到 `androidx.fragment.app`

5. 升级第三方库butterknife版本

    ```
    butterknife 8.8.1 -> 10.0.0
    butterknife-compiler
    ```

6. 需要 java8语言特性，升级java到版本8

    ```
    compileOptions {
        sourceCompatibility JavaVersion.VERSION_1_8
        targetCompatibility JavaVersion.VERSION_1_8
    }
    ```
