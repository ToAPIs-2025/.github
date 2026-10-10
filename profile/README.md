# ToAPIs — AI APIs for developers and production teams

Integrate text, image, and video models into your applications and recurring workflows. Use OpenAI-compatible chat and dedicated image/video APIs with one API key.

**[Get an API key](https://toapis.com/dashboard/tokens?utm_source=github&utm_medium=organic_profile&utm_campaign=gh_org&utm_content=api_key)** · **[Run the Python examples](https://github.com/ToAPIs-2025/toapis-quickstart)** · **[API docs](https://docs.toapis.com/docs/en/quickstart)** · **[Live pricing](https://toapis.com/en/pricing?utm_source=github&utm_medium=organic_profile&utm_campaign=gh_org&utm_content=pricing)** · **[Production integration support](mailto:support@toapis.com?subject=Production%20API%20integration)**

[English](https://github.com/ToAPIs-2025/.github/blob/main/profile/README.md) · [简体中文](https://github.com/ToAPIs-2025/.github/blob/main/profile/README_zh-CN.md) · [日本語](https://github.com/ToAPIs-2025/.github/blob/main/profile/README_ja.md) · [한국어](https://github.com/ToAPIs-2025/.github/blob/main/profile/README_ko.md) · [Русский](https://github.com/ToAPIs-2025/.github/blob/main/profile/README_ru.md)

## Built for recurring API workloads

| Your workload | Where to start |
| --- | --- |
| Integrating models into an app or SaaS | Reuse the OpenAI SDK for compatible chat calls; check model-specific parameters. |
| Producing product images or ad assets in batches | Validate one image task, then build a queue with bounded concurrency and saved task IDs. |
| Running repeated video-generation jobs | Submit a task, query its status, and save the result before the link expires. |
| Migrating an existing API workload | Verify model mapping, response formats, limits, and billing with a small sample first. |

The web playground helps you evaluate outputs. These repositories focus on API integration. The current Python quickstart demonstrates **single requests and asynchronous polling**; batch orchestration belongs in your application.

## Start with a runnable example

Our [Python quickstart](https://github.com/ToAPIs-2025/toapis-quickstart) covers chat, image submission/polling, and video submission/polling without third-party Python packages.

Install Python 3.10+, clone the repository, and inspect a request before making a live call:

```bash
git clone https://github.com/ToAPIs-2025/toapis-quickstart.git
cd toapis-quickstart
python examples/quickstart.py chat --dry-run
python examples/quickstart.py image --dry-run
python examples/quickstart.py video --dry-run
```

Then follow the repository's [key configuration and live-call instructions](https://github.com/ToAPIs-2025/toapis-quickstart#2-get-a-key-and-make-one-live-call). Live calls are billed according to your account's current rates.

## Model coverage and cost planning

| API category | Model families |
| --- | --- |
| Text | GPT, Claude, Gemini, DeepSeek |
| Images | GPT Image, Gemini Image, Seedream, FLUX |
| Video | Sora, Veo, Kling, Seedance |
| Music | [Suno](https://toapis.com/en/model-guide/suno) — see its dedicated guide |

Check the [current catalog](https://toapis.com/en/market?utm_source=github&utm_medium=organic_profile&utm_campaign=gh_org&utm_content=models) for availability and supported parameters. Compare [billing units and live prices](https://toapis.com/en/pricing?utm_source=github&utm_medium=organic_profile&utm_campaign=gh_org&utm_content=cost_planning), test a small sample, and inspect actual charges in Usage Logs before scaling.

## Prepare for sustained or batch usage

- Check model-specific limits and your account's allowed concurrency.
- Save task IDs and results; after an interrupted generation request, inspect its status before resubmitting.
- Handle authentication, parameter, rate-limit, and timeout errors separately.
- Set a workload budget and monitor actual usage as you increase volume.

Start with the [quickstart troubleshooting guide](https://github.com/ToAPIs-2025/toapis-quickstart#troubleshooting) and [API documentation](https://docs.toapis.com/docs/en/quickstart).

## High-volume and enterprise integration

Running sustained usage, moving an existing workload, or preparing a team deployment? [Request 1:1 integration support](mailto:support@toapis.com?subject=Production%20API%20integration).

Include your use case, required models, estimated monthly usage, peak concurrency, launch timeline, and integration blocker. Capacity, commercial terms, and dedicated support scope are assessed for your project.

For API troubleshooting, include the endpoint, model, HTTP status, task/request ID, and a redacted reproduction. Never include API keys. Use repository Issues for reproducible example-code defects; contact support privately for account and billing questions.

[Website](https://toapis.com/en?utm_source=github&utm_medium=organic_profile&utm_campaign=gh_org) · [X @toapisai](https://x.com/toapisai) · [Contact support](mailto:support@toapis.com)
