# error
## 在game窗口里，设置新的分辨率，在编辑器中显示的错误  
```
InvalidOperationException: Operation is not valid due to the current state of the object
System.Collections.Stack.Pop () (at /Users/builduser/buildslave/mono/build/mcs/class/corlib/System.Collections/Stack.cs:329)
UnityEngine.GUILayoutUtility.EndLayoutGroup () (at C:/buildslave/unity/build/Runtime/IMGUI/Managed/GUILayoutUtility.cs:323)
UnityEngine.GUILayout.EndVertical () (at C:/buildslave/unity/build/Runtime/IMGUI/Managed/GUILayout.cs:322)
UnityEditor.HostView.OnGUI () (at C:/buildslave/unity/build/Editor/Mono/HostView.cs:91)
```
* 其实还是不知道什么原因，重启下就好了