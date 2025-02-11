# 虚拟形象粒子系统限制

描述对虚拟形象粒子系统的限制

为了防止滥用和大量使用粒子影响性能，粒子系统在虚拟形象上使用时可能会受到限制。以下是我们在 2018 年 6 月 19 日推荐遵守的的限制。

> 在 Quest 中启用<br>
> 默认情况下，此系统在 Quest 上以默认设置启用，无法被禁用。这是出于性能和安全原因的考虑。

请注意，限制器将防止任何粒子与 PlayerLocal 发生碰撞。只有在禁用限制器的情况下才能禁用此功能。

此功能处于测试阶段。此功能可能会在将来的版本中更改、修改或删除。

我们鼓励用户尝试接触这些设置，以寻找并共享一些允许合法使用粒子系统的设置，而不是那些能够导致性能问题或应用程序崩溃的系统。

## 默认粒子限制器设置

```json
{
	"betas": [
		"particle_system_limiter"
	],
	"ps_max_particles": 50000,
	"ps_max_systems": 200,
	"ps_max_emission": 5000,
	"ps_max_total_emission": 40000,
	"ps_mesh_particle_divider": 60,
	"ps_mesh_particle_poly_limit": 50000,
	"ps_collision_penalty_high": 50,
	"ps_collision_penalty_med": 30,
	"ps_collision_penalty_low": 10,
	"ps_trails_penalty": 10
}
```

## 粒子限制器配置说明

值名称 | 描述
-- | --
`betas` |	添加或删除字符串“particle_system_limiter”将启用/禁用限制器系统
ps_max_particles | 单个粒子系统可以生成的最大粒子数
`ps_max_emission`	| 允许单粒子系统的最大发射量
ps_max_total_emission | 虚拟形象上所有粒子系统之间允许的最大发射
`ps_mesh_particle_divider` | 网格粒子惩罚的计算方法是使用它们中的最高多边形网格除以此值，结果值除以粒子系统的最大粒子余量
ps_mesh_particle_poly_limit	| 在粒子系统上网格的最大多边形数
`ps_collision_penalty_high` | 在粒子系统上高质量碰撞的惩罚，结果值除以粒子系统的最大粒子余量
ps_collision_penalty_med | 在粒子系统上中等质量碰撞的惩罚，结果值除以粒子系统的最大粒子余量
`ps_collision_penalty_low` | 在粒子系统上低质量碰撞的惩罚，结果值除以粒子系统的最大粒子余量
ps_trails_penalty | 在粒子系统上启用尾迹的惩罚，结果值除以粒子系统的最大粒子余量

## 修改 VRChat 粒子限制器配置

如果您愿意，您可以更改粒子限制器系统以获得自己的本地效果。我们仅建议高阶用户更改这些默认设置。

编辑这些值需要重新启动应用程序才能生效。

您可以通过将文件添加到以下目录中来覆盖所有设置或完全禁用限制器系统：

`%AppData%\..\LocalLow\VRChat\vrchat`

按以下方式命名文件：

`config.json`

确保文件扩展名为`json`，而不是`txt`。最好使用 Notepad++ 等编辑器编辑配置文件。

将此页面顶部默认配置的内容复制并粘贴到您的文件中，然后根据自己的心血来潮进行编辑！例如，您可以增加 `ps_max_particles` 以允许每个单独的系统使用更多粒子，或者从`beta`部分删除字符串 `ps_max_particles"particle_system_limiter"` 以完全禁用系统而不删除文件。

## 预填充的默认配置文件

您还可以在[此处](https://assets.vrchat.com/misc/vrchat%3Bconfig.json)下载预填充了默认配置的文件。如果单击文件时显示而不是下载文件，请右键单击链接，单击“另存为”，然后下载它。必须将文件重命名为 `config.json` 。将文件放入上面指定的目录 （`%AppData%\..\LocalLow\VRChat\vrchat`），您就可以开始了。请记住，必须精确命名文件为 `config.json`。