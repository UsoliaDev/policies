# 游戏翻译器

?> **实验性功能**：使用中可能会出现问题，请将其反馈给我们以便于改善该功能：[错误反馈](https://usolia.net/bug-report)

> 该功能目前仅可在 Creative Land II (cl02) 和 Planet (pl0x) 服务器上使用。

*语言不通？鸡同鸭讲？这些不再成为问题。*

*本文最后更新于 2023.7.21*

------

## 简介

这是一个由 OpenAI 的 GPT-3.5-turbo 模型提供支持的翻译器，支持将大部分语言翻译为你所指定的语言。在将来我们可能会引入更多翻译提供商，例如 DeepL。

!> 翻译过程中，你的文本将被发送到 Usolia Network 外部以进行翻译。详情查看下方“数据隐私”一节。

## 使用

### 1.启动翻译

在服务器内输入指令 `/translate <lang-code>` 启动翻译，将你在下一步时输入的文本翻译为 `<lang-code>` 部分中指定的语言。

`<lang-code>` 部分可以是以下值：

- `de_de` | 德语
- `en_us` | 英语（美式）
- `es_es` | 西班牙语
- `fr_fr` | 法语
- `it_it` | 意大利语
- `ja_jp` | 日语
- `ru_ru` | 俄语
- `zh_cn` | 简体中文

### 2. 输入翻译文本

完成第一步后，服务器会提示你输入需要翻译的文本。

将你需要翻译的文本直接输入在聊天栏并发送即可，服务器将把翻译后的文本发送回你。如果不慎选择了错误的语言，你可以输入“cancel”以取消翻译。

你可以点击以将翻译后的文本粘贴到聊天栏，如下图所示：

![translator-1](https://usolia.net/img/docs/mechanisms/translator-1.png)

## 数据隐私

翻译服务由 Azure OpenAI 服务提供，提交文本以进行翻译时你的以下信息将被发送到 Azure 服务器：

- 你指定翻译的文本

以下页面阐述了 Azure OpenAI 服务将如何处理你的数据：

[# Data, privacy, and security for Azure OpenAI Service](https://learn.microsoft.com/en-us/legal/cognitive-services/openai/data-privacy)

如果你不接受其使用你的数据，则请勿使用该游戏翻译器功能。