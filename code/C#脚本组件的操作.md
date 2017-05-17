# C#脚本组件的操作
在C#脚本中对组件的动态操作，如：组件的加载、获取、激活、删除等
```c#
// 用两个C#脚本组件，MyComponent 和 MyComponent1
// 其中 MyComponent 在编辑器中直接挂载在，GameObject上
// 挂载一个 MyComponent1 组件
gameObject.AddComponent<MyComponent1>();
// 获取 gameObject 上的一个组件
MyComponent1 mc =  gameObject.GetComponent<MyComponent1>();
if (mc)
{
    Debug.Log("组件被加载了");
}
// 禁用组件
mc.enabled = false;
// 删除 Component 组件
Destroy(mc);
if (mc)
{
    Debug.Log("删除成功"); // 删除成功执行这个
}
else
{
    Debug.Log("删除失败");
}
```