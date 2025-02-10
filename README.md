# 组件总目录

01. 标题栏：TitleBar
02. 大标题：ItemOuterLargeTitle
03. 圆角列：RoundedColumn
04. 复选框：ItemCheck
05. 按钮：ItemButton
06. 标题：ItemTitle
07. 标准项：Item
08. 开关：ItemSwitcher
09. 提示：ItemTip
10. 信息：ItemInfo
11. 值：ItemValue
12. 输入框：ItemEdit
13. 密码框：ItemEditPassword
14. 弹出菜单：ItemPopup
15. 对话框：YesNoDialog, YesDialog, InputDialog
16. 滑块：ItemSlider
17. 底部栏：BottomBar
18. 底部栏项：BottomBarItem

---

## 1. 标题栏：TitleBar


```kotlin
TitleBar(
    onBack = { /* 返回按钮回调 */ },
    text = "标题"
)
```

---

## 2. 大标题：ItemOuterLargeTitle

```kotlin
ItemOuterLargeTitle(
    text = "大标题",
    sub = "副标题"
)
```

---

## 3. 圆角列：RoundedColumn

```kotlin
RoundedColumn {
    // 内部放置其他组件
}
```

---

## 4. 复选框：ItemCheck

![Alt text](Pictures/ItemCheck.png)
```kotlin
ItemCheck(
    state =false, //开关启用状态
    onChange = { /* 状态改变回调 */ },
    text = "复选框"
)
```

---

## 5. 按钮：ItemButton

```kotlin
ItemButton(
    onClick = { /* 点击回调 */ },
    text = "按钮"
    primary = false//强调色状态
)
```

---

## 6. 小标题：ItemTitle

```kotlin
ItemTitle(text = "标题")
```

---

## 7. 标准项：Item

```kotlin
Item(
   onClick = {},
  // iconPainter = painterResource(R.drawable.ic_qr_code),
  // iconColor = SaltTheme.colors.highlight,
   text = "标准 Item 控件，带图标（可选），副标题文本（可选）",
   sub = "Item 控件的副标题"
                )
```

---

## 8. 开关：ItemSwitcher
![Alt text](Pictures/ItemSwitcher.png)
```kotlin
ItemSwitcher(
    state = false,
    onChange = { /* 状态改变回调 */ },
    text = "开关"
)
```

---

## 9. 提示：ItemTip
![Alt text](Pictures/ItemTip.png)
```kotlin
ItemTip(text = "提示信息")
```

---

## 10. 信息：ItemInfo
![Alt text](Pictures/ItemInfo.png)
```kotlin
ItemInfo(
    text = "警告信息",
    infoType = ItemInfoType.Warning
)
```

---

## 11. 值：ItemValue
<img src="Assets/S50208-01534347_com.moriafly.salt.ui_z8zf.png" width="1080"></img>
```kotlin
ItemValue(
    text = "标题",
    sub = "内容"
)
```

---

## 12. 输入框：ItemEdit
![Alt text](Pictures/ItemEdit.png)
```kotlin
ItemEdit(
    text = "",
    onChange = { /* 文本改变回调 */ },
    hint = "输入框提示"
)
```

---

## 13. 密码框：ItemEditPassword
![Alt text](Pictures/ItemEditPassword.png)
```kotlin
ItemEditPassword(
    text = "",
    onChange = { /* 文本改变回调 */ },
    hint = "密码输入框提示"
)
```

---

## 14. 弹出菜单：ItemPopup

```kotlin
ItemPopup(
    state = popupState,
    text = "弹出菜单",
    sub = "副标题"
) {
    PopupMenuItem(
        onClick = { /* 点击回调 */ },
        text = "选项一"
    )
}
```

---

## 15. 对话框：YesNoDialog, YesDialog, InputDialog

```kotlin
YesNoDialog(
    onDismissRequest = { /* 关闭回调 */ },
    onConfirm = { /* 确认回调 */ },
    title = "对话框标题",
    content = "对话框内容"
)

YesDialog(
    onDismissRequest = { /* 关闭回调 */ },
    title = "对话框标题",
    content = "对话框内容"
)

InputDialog(
    onDismissRequest = { /* 关闭回调 */ },
    onConfirm = { /* 确认回调 */ },
    title = "输入对话框标题",
    text = "",
    onChange = { /* 文本改变回调 */ }
)
```

---

## 16. 滑块：ItemSlider
<img src="Assets/S50208-01553905_com.moriafly.salt.ui_g4ou.png" width="1080"></img>
```kotlin
ItemSlider(
    value = 0f,
    onValueChange = { /* 值改变回调 */ },
    text = "滑块"
)
```

---

## 17. 底部栏：BottomBar

```kotlin
BottomBar {
    BottomBarItem(
        state = true,
        onClick = { /* 点击回调 */ },
        painter = painterResource(Res.drawable.ic_qr_code),
        text = "底部栏项"
    )
}
```

---

## 18. 底部栏项：BottomBarItem

```kotlin
BottomBarItem(
    state = true,
    onClick = { /* 点击回调 */ },
    painter = painterResource(Res.drawable.ic_qr_code),
    text = "底部栏项"
)
```

---