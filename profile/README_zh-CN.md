# ToAPIs — 面向开发者与生产团队的 AI API

将文本、图像和视频模型接入你的应用与持续生产流程。文本调用兼容 OpenAI SDK，图像和视频使用专用接口，通过一个 API Key 接入。

**[获取 API Key](https://toapis.com/dashboard/tokens?utm_source=github&utm_medium=organic_profile&utm_campaign=gh_org&utm_content=api_key_zh)** · **[运行 Python 示例](https://github.com/ToAPIs-2025/toapis-quickstart/blob/main/README_zh-CN.md)** · **[API 文档](https://docs.toapis.com/docs/cn/quickstart)** · **[当前价格](https://toapis.com/pricing?utm_source=github&utm_medium=organic_profile&utm_campaign=gh_org&utm_content=pricing_zh)** · **[生产接入咨询](mailto:support@toapis.com?subject=Production%20API%20integration)**

[English](https://github.com/ToAPIs-2025/.github/blob/main/profile/README.md) · [简体中文](https://github.com/ToAPIs-2025/.github/blob/main/profile/README_zh-CN.md) · [日本語](https://github.com/ToAPIs-2025/.github/blob/main/profile/README_ja.md) · [한국어](https://github.com/ToAPIs-2025/.github/blob/main/profile/README_ko.md) · [Русский](https://github.com/ToAPIs-2025/.github/blob/main/profile/README_ru.md)

中国境内访问可使用 [toapis.cn](https://toapis.cn) 和 [docs.toapis.cn](https://docs.toapis.cn/)。以下示例默认使用国际站，切换方法见快速接入仓库。

## 面向持续 API 调用的场景

| 你的需求 | 接入路径 |
| --- | --- |
| 为应用或 SaaS 接入模型 | 兼容的文本调用沿用 OpenAI SDK，并核对模型参数。 |
| 批量生产商品图或广告素材 | 先验证一个图像任务，再在业务系统中加入队列、并发控制和任务记录。 |
| 持续提交视频生成任务 | 提交任务、查询状态，及时保存结果。 |
| 迁移已有 API 用量 | 用小样本核对模型映射、返回格式、调用限制和计费。 |

网页试用用于验证生成效果；GitHub 示例重点服务 API 接入。现有 Python 快速开始提供**单次调用和异步任务查询**，批量调度需要在你的业务系统中实现。

## 从可运行的示例开始

[Python 快速接入仓库](https://github.com/ToAPIs-2025/toapis-quickstart/blob/main/README_zh-CN.md)包含文本调用、图像任务和视频任务的提交与查询，无需安装第三方 Python 包。

安装 Python 3.10 或更新版本，克隆仓库，先检查请求参数：

```bash
git clone https://github.com/ToAPIs-2025/toapis-quickstart.git
cd toapis-quickstart
python examples/quickstart.py chat --dry-run
python examples/quickstart.py image --dry-run
python examples/quickstart.py video --dry-run
```

再按仓库说明配置环境变量中的 API Key，完成一次正式调用。正式调用按账户当前价格计费。

## 模型覆盖与成本评估

| 接口类别 | 模型系列 |
| --- | --- |
| 文本 | GPT、Claude、Gemini、DeepSeek |
| 图像 | GPT Image、Gemini Image、Seedream、FLUX |
| 视频 | Sora、Veo、Kling、Seedance |
| 音乐 | [Suno](https://toapis.com/en/model-guide/suno)，使用专用指南 |

在[模型目录](https://toapis.com/market?utm_source=github&utm_medium=organic_profile&utm_campaign=gh_org&utm_content=models_zh)核对当前可用模型和参数。先比较[计费单位与当前价格](https://toapis.com/pricing?utm_source=github&utm_medium=organic_profile&utm_campaign=gh_org&utm_content=cost_planning_zh)，用小样本验证，并通过 Usage Logs 核对实际消耗，再扩大调用量。

## 持续调用与批量生产前的准备

- 核对模型限制和账户允许的并发量。
- 保存任务 ID 和结果；生成请求中断后先查询原任务，再决定是否重新提交。
- 分别处理认证、参数、限流和超时错误。
- 设置业务预算，扩大调用量时持续检查实际用量。

基础问题先查[示例仓库排错说明](https://github.com/ToAPIs-2025/toapis-quickstart/blob/main/README_zh-CN.md)与 [API 文档](https://docs.toapis.com/docs/cn/quickstart)。

## 高用量与企业级接入咨询

有持续用量、已有业务迁移或团队上线需求，可[申请 1V1 接入支持](mailto:support@toapis.com?subject=Production%20API%20integration)。

请提供业务场景、所需模型、预计月用量、峰值并发、上线时间和当前接入问题。我们根据项目需求评估容量、商务条件和专属支持范围。

API 排错请提供接口、模型、HTTP 状态、任务或请求 ID 及脱敏复现信息，不要提供 API Key。示例代码缺陷可提交仓库 Issue；账户和账单问题请私下联系支持。

[官网](https://toapis.com?utm_source=github&utm_medium=organic_profile&utm_campaign=gh_org) · [X @toapisai](https://x.com/toapisai) · [联系支持](mailto:support@toapis.com)
