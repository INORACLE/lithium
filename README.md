# Lithium (Forge 1.20.1)

Lithium 是一个提升 Minecraft 游戏性能的模组，通过优化各种游戏机制（AI、寻路、区块逻辑、碰撞检测、红石等）来显著减少 CPU 开销，且不改变游戏玩法。

本仓库包含 **Radium** — Lithium 的 Forge 移植版本，目标版本为 **Minecraft 1.20.1 / Forge**。

> 注意：Lithium 本身是 Fabric 模组，Fabric 与 Forge 使用不同的模组加载器和 API。本仓库使用社区移植项目 [Radium](https://github.com/Reforged-Hub/radium-upstream)（Radium Reforged）的 1.20.1 分支，用于构建 Forge 版本。

## 环境要求

- Java 17（JDK 17）
- Minecraft 1.20.1
- Forge 47.1.3

## 构建

```bash
./gradlew build
```

构建产物位于 `build/libs/`。

## GitHub Actions

仓库已配置 CI 工作流（`.github/workflows/build.yml`），每次推送到 `main` 或创建 Pull Request 时自动：

1. 使用 JDK 17 在 Ubuntu 环境执行 `./gradlew build`
2. 将 `build/libs/*.jar` 上传为构建 artifact

构建产物可在 GitHub 仓库的 **Actions** 页面下载。

## 许可

本仓库内容基于 [Radium](https://github.com/Reforged-Hub/radium-upstream) 的 1.20.1 分支，遵循 [GNU Lesser General Public License v3.0](LICENSE.txt)。