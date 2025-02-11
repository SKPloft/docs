# Valve Index 控制器

VRChat 支持 Valve Index 控制器！

## 手指姿态

Valve Index 控制器包含了小拇指、无名指和中指的电容传感器用于检测这三根手指的姿态。它还有着扳机上的食指电容传感器和触摸板/按键上的传感器用于检测您的大拇指是否被“按下”。最后，它还包含了一个压力传感器来检测用户是否紧握着控制器。

在 VRChat 中，角色的形象会实时跟踪控制器上手指的姿态。尽管追踪不完全精确,但手指的开合状态仍可以反映到您的形象手上，提升沉浸感。

## 手势切换

当您启用手势切换时， VRChat 将尝试将您当前的手指姿势与[标准 VRChat 手部姿势](../../blank.md)相匹配。任何指定的手势动画都会被触发，*但即使您为手的位置定义了一个手势动画,您的手势也不会自动改变。*

当您禁用手势切换时，VRChat 将不会尝试匹配手势。

如果您在触发一个手势动画时关闭手势切换，那个手势动画会继续播放，直到您再次启用手势切换。

## 物体交互

抓取物体(比如 Battle Discs 中的盘子)是通过握紧手柄来完成的。松开握持会让物体掉落。使用 Valve Index 手柄可以让像 Battle Discs 这样的游戏感觉更沉浸和自然。握持力度的要求可以和许多其他设置一起进行调整。

## 设置默认的键位绑定

请确保您在 SteamVR `设置>控制器绑定>VRChat`中为 Index 控制器使用“VRChat bindings for Index Controller”。这一点非常重要--如果您正在使用 Index 控制器的旧自定义设置，它们将无法正常工作！

SteamVR 控制器绑定页面可能有点 bug ，所以确保在您选择绑定后它们已正确设置。

这些绑定已经被设置为 VRChat 的“默认绑定”。您可以在 SteamVR 控制器设置中找到它们。不过您可能需要在 SteamVR 中使用“使用旧版绑定界面（Use Old Binding UI）”按钮。

您也可以在 SteamVR 控制器绑定菜单中调整多种设置，包括抓取所需的力度。如果您觉得有些东西不对劲，也可以选择调整这些设置。如果您找到了自己喜欢的设置方案，您可以使用 SteamVR 将这些绑定方案共享给其他人！

![img](../../img/valve-index-1.png)

<center>

*如果闭合您的小拇指/无名指/中指有点困难，您可以试着在握持绑定上的“保持力度（Force Hold）”和“释放力度（Force Release）”设置中将值调低。*

</center>

## 自定义绑定说明

- 在重新分配"可触摸的拇指"按钮触摸事件时要小心。VRChat 会检查拇指可以触摸的每个按钮的触摸事件，来判断拇指是否弯曲。如果一个"可触摸的拇指"按钮没有被分配相同的触摸事件，VRChat 就无法判断拇指是否已经弯曲，这将导致追踪不准确。

- `跳跃`，`麦克风切换`，`手势切换`以及`动作菜单左/右`都是对应用程序的硬输入绑定。

## VRChat标准手势

手势名称 | 手势描述
-- | --
握拳 | 小拇指、无名指和中指闭合<br>食指放在扳机上<br>大拇指闭合
张开手 | 小拇指、无名指和中指抬起<br>食指离开扳机<br>大拇指抬起向
指向 | 小拇指、无名指和中指闭合<br>食指离开扳机<br>大拇指闭合
竖大拇指 | 小拇指、无名指和中指闭合<br>食指放在扳机上<br>大拇指抬起
剪刀手 | 小拇指、无名指闭合，中指抬起<br>食指离开扳机<br>大拇指闭合
手枪 | 小拇指、无名指和中指闭合<br>食指离开扳机<br>大拇指抬起
摇滚 | 小拇指抬起，无名指和中指闭合<br>食指离开扳机<br>大拇指闭合

## 按键分配

按键 | 效果
-- | --
右侧A（右侧手柄底部按键） | 跳跃
左侧A（左侧手柄底部按键） | 静音
B（手柄顶部按键） | 快捷菜单<br>行动菜单（按住）
触摸板触摸 | *为未来的特性保留（目前无效果）*
触摸板按下 | *为未来的特性保留（目前无效果）*
触摸板滑动 | *为未来的特性保留（目前无效果）*
握持 | 捡起
扳机 | 选择/交互
右摇杆 | 转向
左摇杆 | 移动
右摇杆下压  | 右侧[动作菜单](./action-menu.md)
左摇杆下压  | 左侧[动作菜单](./action-menu.md)

## 绑定说明

VRChat 使用 Unity 的 Mechanim 和 Mixamo 的"YBot"角色作为标准的绑定设置。您可能会发现，随着手指灵巧性的提高，模型对手部绑定的要求也增加了，您可能需要调整绑定和绘制权重。一个用于测试的好方法是使用 Unity 的[ Avatar Muscles 和 Settings 选项卡](https://docs.unity3d.com/Manual/MuscleDefinitions.html)来测试手部的张开/闭合状态。如果手部姿势看起来有些奇怪，您可能需要稍微调整您的权重绘制和绑定设置。
