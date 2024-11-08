
**Show Build Duration**
```shell
defaults write com.apple.dt.Xcode ShowBuildOperationDuration YES
```

**Clean Derived Data**
```shell
rm -rf ~/Library/Developer/Xcode/DerivedData
```

**Kill Xcode**
```shell
killall xcode
```

**Validate Plist for Syntax Error**
```shell
plutil -lint Info.plist
```

**List Code Signing Certificates**
```shell
security find-identity -v -p codesigning
```

**Customize Simulator Status Bar**
```shell
xcrun simctl status_bar "iPhone 14" override --time "9:41" --dataNetwork wifi --wifi-mode active --cellular-mode active
```

**Reset Simulator**
```shell
xcrun simctl erase all
```

**List Simulator Device**
```shell
xcrun simctl list
```
