# ResourceManager
> 基于 `Unity引擎` 的游戏开发框架以及通用技术模型，致力于各模块技术模型各自独立，零耦合设计。

## `ResConfig`

>  - `CurLoadModel`  = 当前加载资源的模式
>  > 0. Resources
>  > 0. AssetBundle
>  > 0. AssetBundleSimulation（该模式应用于Editor下模拟AB加载的方式）


----

> - `ResFolderPath` = 资源根目录

> - `EmptyRunLimit` = 休闲待机次数
> 待补充

> > 默认 `1000` 次。当休闲次数超过当前设定时，加载模块会自动停止 `Loop` 状态。

## 环境初始化

> - 在主线程里调用 `InitResourceEnv` 来初始化加载环境。

> > 如果是 `AssetBundle` 模式，在调用 `InitResourceEnv` 之后，还需调用 `InitAssetBundleManifest` 来初始化 `Manifest`。
> 待补充
