# 概述
* GameObject 实体、节点
* Component 组件
* GameObject 和 Component 的关系  
  和人跟衣服的关系类似，人是GameObject，衣服是Component，不同的衣服在人身上表示着不同的身份，校服意味着这个人是学生，警服意味着这个人是警察……
# GameObject
* 不承担行为
* 通用属性  
    |属性名 |说明|
    |:----:|:---|
    |tags  | 为节点添加一个tag，可以在游戏中获取到所有被指定为 这个tags 的所有 GameObject，通常在游戏中比较少使用，应为查找的成本比较高|
    |static|与优化相关，在游戏中不变的要素，对于建筑就可以设置这个属性|
# Component
* 负责行为逻辑
* 组件的设计应该是独立的，最好不要针对某种特定的 GameObject
* Transform 所有的节点都必须有的组件，代表，位置、旋转、缩放
* 分类
    * 内置组件
    * 自定义组件
* 组件的创建
    * 组件的名字和C#的类名一样
    * 能作为组件的脚本，都必须要继承自 MonoBehaviour 类
    * 把组件属性暴露给 Inspector 编辑