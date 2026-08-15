<br><br>

<h1 align = "center">Photon GAMS（透明修复版）</h1>

<p align = "center">在 Photon GAMS 基础上修复“半透明贴图不显示”问题的个人修复分支</p>

## 本分支修复了什么

原版 Photon GAMS 存在一个 bug：粒子（药水粒子、篝火烟雾等）和生物实体上的半透明贴图（例如灾变模组的咒翼灵骸）完全不显示，或显示成“比空气更透明”的轮廓。

本分支参照 Photon GAMS PLUS 的渲染方式，修复了 `gbuffers_all_translucent` 的 alpha 处理，使透明粒子与半透明实体正常显示，同时保留 GAMS 版的其它全部特性与默认观感。

> 提示：修复后原版雨粒子会正常可见（原版 GAMS 中它们只是被 bug 隐藏了）。如果不希望看到粒子雨，可搭配 Particle Rain（粒子雨）模组使用，效果更佳。

## 安装

1. 下载本仓库 ZIP（或 Release 中的 zip 文件）。
2. 将 zip 放入 Minecraft 的 `shaderpacks` 文件夹（OptiFine / Iris / Oculus 均可）。
3. 在游戏内 选项 → 光影/画质 中选中 Photon GAMS（透明修复版）。

## 与原版的差异

仅修改了半透明/粒子相关的 alpha 处理逻辑，其余着色器文件与设置均与原版 Photon GAMS 保持一致。

---

<h1 align = "center">Photon GAMS</h1>

<p align = "center">A gameplay-focused shader pack for Minecraft based on Photon by Sixthsurge</p>

![Screenshot](docs/images/a.png)

## Acknowledgments

* OUdefie17 (Mod support, Colored Light settings, Some features)
* Arona74  (Mod support, Transfer to new versions of Photon, Owner of the dev branch)
* -Daytendo64- (Galaxy, Nebula, Shooting Stars, End Solar Flare settings)
* sw-52 (More Tonemap Operators and settings, Fog settings, DOF settings)

## Features

* Better Hardcoded Emission
* More customization options
* More settings for Colored Light, Water, Sky, Fog
* Better supprort for mods
* More Tonemap Operators

## Community

For questions, suggestions and news regarding this shader pack, head to [Photon discord server thread](https://discord.com/channels/1007736612488220724/1288402151097499698)

## License

基于 [Photon Shaders](https://github.com/sixthsurge/photon)（作者 SixthSurge）与 Photon GAMS。请遵守随附的 LICENSE 条款：可免费重新分发修改版，但不得在 CurseForge / Modrinth 等有收益平台发布，不得收费。
