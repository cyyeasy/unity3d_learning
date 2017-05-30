# 最基本的window
在unity编辑器中，创建一个自定义的编辑器
## 代码
```c#
using UnityEditor; // 需要包含进这个名字空间
using UnityEngine;

public class MyWindow : EditorWindow {

    string myString = "Hello Unity Editor";
    // 添加自定窗口在 window/MyWindow 中启动
    [MenuItem("Window/MyWindow")]
    public static void ShowWindow()
    {
        // 如果编辑器中不存在一个MyWindow的实例，那么将创建一个
        EditorWindow.GetWindow(typeof(MyWindow));
    }
    // 用于绘制窗口所有的控件
    void OnGUI()
    {
        GUILayout.Label(myString, EditorStyles.boldLabel);
    }
}
```
## 打开这个窗口
unity菜单 **window** --> **MyWindow**  
![打开MyWindow窗口](../assets/editor_mywindow1.png)

## 显示的界面
![显示的界面](../assets/editor_mywindow2.png)