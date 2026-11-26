# 大肥鱼桌宠 · 形象包素材

[大肥鱼桌宠](https://github.com/shenliuyu18/dafeiyu-pet) 的按需下载形象包。素材放在 Release 资产里，避免 100MB+ 的动画包占用源码仓库。

## 下载

当前 Release：[Character pack 1.0.1](https://github.com/shenliuyu18/dafeiyu-pet-assets/releases/tag/packs-1.0.1)

每个形象提供两种规格：

- **完整版**：640×360 VP9 透明 WebM，CRF 32 + sharpness 2 + cpu-used 2
- **Lite**：480×270 VP9 透明 WebM，CRF 42，供 Lite 版应用自动选择

应用内下载会自动探测直连与 ghfast / gh-proxy / ghproxy 等镜像的速度，优先走最快线路，失败时自动切换。

| 形象 | 资产前缀 | 完整版 | Lite | 动作数 |
| --- | --- | ---: | ---: | ---: |
| 大肥鱼 plus | `dsh1-` | 193.1 MiB | 49.4 MiB | 167 |
| GPT娘v1 | `gptv1-` | 2.2 MiB | 2.2 MiB | 1（73 帧图集） |
| GPT娘v2 | `gptv2-` | 97.0 MiB | 21.1 MiB | 92 |
| Claude 动作包 | `claude-` | 113.2 MiB | 24.3 MiB | 166 |
| Gemini 动作包 | `gemini-` | 82.2 MiB | 18.3 MiB | 100 |
| GLM 动作包 | `glm-` | 86.5 MiB | 19.5 MiB | 97 |
| Grok 动作包 | `grok-` | 89.1 MiB | 21.1 MiB | 106 |
| Kimi 动作包 | `kimi-` | 72.0 MiB | 18.3 MiB | 105 |
| Qwen 动作包 | `qwen-` | 79.9 MiB | 19.3 MiB | 106 |

完整版合计约 815.0 MiB，Lite 合计约 193.4 MiB。

安装：在应用「设置 → 形象与音效」里按需下载；也可以下载 zip 后从「导入形象包」安装。包内是标准 `manifest.json` + 动画文件，格式见[形象包制作标准](https://github.com/shenliuyu18/dafeiyu-pet/blob/main/docs/形象包制作标准.md)。

## 校验

```bash
sha256sum -c SHA256SUMS.txt
```

## 许可与署名

本仓库只做格式转换与重新编码，不主张角色或动画的版权。各包的来源与授权如下：

- **GPT娘v1**（`gptv1-`）：73 帧透明图集来自 [weit0529/gpt-pet](https://github.com/weit0529/gpt-pet)（MIT）。
- **大肥鱼 plus**（`dsh1-`）：动作来自 [hunmer/aboutme-pets](https://github.com/hunmer/aboutme-pets) 的 dsh1 动作包（上游作者生成），基础形象来自 [PC2005-cloud/dsh-pet](https://github.com/PC2005-cloud/dsh-pet)。上游明确说明：**dsh 系列素材禁止商用，公开二创须署名上游仓库。**
- **GPT娘v2、Claude、Gemini、GLM、Grok、Kimi、Qwen**：动画来自 [hunmer/aboutme-pets](https://github.com/hunmer/aboutme-pets)，基础立绘来自 [lokicorvus/crosspet](https://github.com/lokicorvus/crosspet)，按 [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/) 署名、非商业、相同方式共享。本仓库的转码版本按相同条件提供。

以上授权不允许商业使用；商业授权需分别联系上游作者与立绘权利人。若权利人认为本仓库的再分发不妥，请在[主仓库 Issues](https://github.com/shenliuyu18/dafeiyu-pet/issues) 说明，我们会及时下架。