## To create Icons for mac app, follow these steps. 
1. Go to https://appicon.co/ and select macOS.
2. Upload 1024x1024px png image and download the generated zip file. 
3. The zip file contains the Assets.xcassets folder. 
4. On mac machine execute this command to generate Assets.car and AppIcons.icns files. 
    ```
    xcrun actool Assets.xcassets --compile build --platform macosx --minimum-deployment-target 8.0 --app-icon AppIcon --output-partial-info-plist build/partial.plist
    ```
5. Copy Assets.car and AppIcons.icns files to src/osx/zzv.app/Resources