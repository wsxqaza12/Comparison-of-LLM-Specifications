# AI Language Models Overview

## Introduction
Welcome to this comprehensive overview of the current landscape of AI language models. This document is designed to be a living resource that captures the specifications and release details of various large-scale language models developed by leading technology companies.

The aim is to provide a centralized, up-to-date comparison of these models, which range from OpenAI's GPT series to Google's offerings and beyond. For researchers, developers, and enthusiasts, this comparison serves as a quick reference to understand the capabilities, structures, and unique features of each model.

## Language Models
In this section, we delve into each company's contributions to the field of AI language models. We outline the models they have released, specifying parameters such as model size, underlying structures, training data, token output capacity, context window, type (whether open source or closed source), and release dates.

Understanding these details is crucial for anyone interested in the technical aspects of AI development or looking to leverage these models for various applications.

## Data Integrity and Contributions
In the fast-paced domain of AI, information can quickly become outdated. To maintain the integrity of this repository, we rigorously source and verify any uncertain data before inclusion. Every piece of information is accompanied by a citation linking to its source, ensuring transparency and reliability.

Your insights and updates are crucial to the resource's vitality. We invite you to contribute by submitting pull requests with verifiable information or by flagging any discrepancies you may encounter. Open an issue to discuss potential changes or to seek clarification on existing data.

---

# Comparison-of-LLM-Specifications
| Company    | Model              | Parameters Size           | Structure           | Training Data (Date) | Output Token | context window         | Type       | Release Date |
|------------|--------------------|---------------------------|---------------------|----------------------|--------------|------------------------|------------|--------------|
| OpenAI     | GPT-3.5            | 20B                       | Transformer         | 45T tokens(~2021/09)       | 4,096        | 4k~16k                 | close      | 2022/3/15    |
|            | GPT-4              | 8*220B (Plus, Team, Enterprise) | MoE (8 experts) | ?                  | 4,096        | 32k (Plus, Team) 128K(Enterprise) | close | 2023/4/4  |
| Google     | PaLM 2             | 340B (Unicorn, Bison, Otter, Gecko) | Transformer | 3.6T tokens(~2023/8)   | 1024~8192    | 8K~32K                 | close      | 2023/5/10    |
|            | Gemma              | 2B, 7B                     | Transformer         | 2T, 6T tokens        | ?            | 8K                     | open source | 2024/2/21 |
|            | Gemini 1.0         | Nano1(1.8B), Nano2(3.3B), Pro, Ultra | Transformer | ?                 | 2,048        | 8K                     | close      | 2024/2/8    |
|            | Gemini 1.5         | Pro                        | MoE                 | ?                    | 8,192        | 128k~1m                | close      | 2024/2/15   |
| Anthropic  | Claude 2.1         | 200B                       | Evolved Transformer | ? (~2023/Early)     | 4,096        | 200K                   | close      | 2023/11/21  |
|            | Claude 3           | 20B, 70B, 2T (Haiku, Sonnet, Opus ) | Sparse Transformer | 40T tokens(~2023/8) | 4,096   | 200K                | close      | 2024/3/4    |
| Meta       | Llama2             | 7B, 13B, 70B               | Transformer         | 2T tokens            | 4,096         | 4,096                  | open source | 2023/7/18 |
| Mistral AI | Mistral (Tiny)     | 7B                         | Transformer         | ?                    | ?            | 32k                    | open source | 2023/9/27 |
|            | Mixtral 8x7B (Small) | 45B(use 12B)             | SMoE (8 experts)    | ?                    | ?            | 32k                    | open source | 2023/12/11 |
|            | Mistral            | Medium, Large              | ?                   | ?                    | ?            | 32k                    | close      | 2024/2/26   |


# Details and Rumor sources
### OpenAI
- **GPT-3.5**
  - Parameters Size: 20B?
    - [OpenAI Community](https://community.openai.com/t/how-many-parameters-does-gpt-3-5-have/648417/4)
  - Structure: Transformer
  - Training Data (Date): 45T (~2021/09)?
    - [OpenAI Community](https://community.openai.com/t/what-is-the-size-of-the-training-set-for-gpt-3/360896)
  - Output Token: 4,096
    - [OpenAI Documentation](https://platform.openai.com/docs/models/gpt-3-5-turbo) 
  - Context Window: 4k~16k
    - [OpenAI Documentation](https://platform.openai.com/docs/models/gpt-3-5-turbo) 
  - Type: close
  - Release Date: 2022/3/15

- **GPT-4**
  - Parameters Size: 8*220B? (Plus, Team, Enterprise)
    - [X-Soumith Chintala](https://twitter.com/soumithchintala/status/1671267150101721090?s=46&t=dUCVh9akIWxxNUIkrDJwJg)
  - Structure: MoE (8 experts)
    - [semianalysis](https://www.semianalysis.com/p/gpt-4-architecture-infrastructure)
  - Training Data (Date): ?
  - Output Token: 4,096
    - [OpenAI Documentation](https://platform.openai.com/docs/models/gpt-4-and-gpt-4-turbo)
  - Context Window: 32k (Plus, Team) 128K(Enterprise)
    - [OpenAI Documentation](https://platform.openai.com/docs/models/gpt-4-and-gpt-4-turbo)
  - Type: close
  - Release Date: 2023/4/4

### Google
- **PaLM 2**
  - Parameters Size: 340B? (Unicorn, Bison, Otter, Gecko)
    - [Sundar Pichai](https://www.cnbc.com/2023/05/16/googles-palm-2-uses-nearly-five-times-more-text-data-than-predecessor.html)
  - Structure: Transformer
  - Training Data (Date): 3.6T (~2023/8)?
    - [Sundar Pichai](https://www.cnbc.com/2023/05/16/googles-palm-2-uses-nearly-five-times-more-text-data-than-predecessor.html)
  - Output Token: 1024~8192
    - [Google Documentation](https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models)
  - Context Window: 8K~32K
    - [Google Documentation](https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models)
  - Type: close
  - Release Date: 2023/5/10

- **Gemma**
  - Parameters Size: 2B, 7B
  - Structure: Transformer
  - Training Data (Date): 2T, 6T tokens
    - [DeepMind Report](https://storage.googleapis.com/deepmind-media/gemma/gemma-report.pdf)
  - Output Token: ?
  - Context Window: 8K
    - [Amazon Blog](https://aws.amazon.com/tw/blogs/machine-learning/gemma-is-now-available-in-amazon-sagemaker-jumpstart/)
  - Type: open source
    - [Hugging Face](https://huggingface.co/google)
  - Release Date: 2024/2/21

- **Gemini 1.0**
  - Parameters Size: Nano1(1.8B), Nano2(3.3B), Pro, Ultra
  - Structure: Transformer
  - Training Data (Date): ?
  - Output Token: 2,048
    - [Google Documentation](https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models)
  - Context Window: 8K
    - [Google Documentation](https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models)
  - Type: close
  - Release Date: 2024/2/8

- **Gemini 1.5**
  - Parameters Size: Pro
  - Structure: MoE
    - [Google Blog](https://blog.google/technology/ai/google-gemini-next-generation-model-february-2024/#gemini-15)
  - Training Data (Date): ?
  - Output Token: 8,192
    - [Google Documentation](https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models)
  - Context Window: 128k~1m
    - [Google Documentation](https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models)
  - Type: close
  - Release Date: 2024/2/15

### Anthropic
- **Claude 2.1**
  - Parameters Size: 200B?
    - [claudeai](https://claudeai.uk/anthropic-introduces-claude-2-1-with-200k-context/#google_vignette)
  - Structure: Evolved Transformer
  - Training Data (Date): ? (~2023/Early)
    - [Anthropic Documentation](https://docs.anthropic.com/claude/docs/models-overview)
  - Output Token: 4,096
    - [Anthropic Documentation](https://docs.anthropic.com/claude/docs/models-overview)
  - Context Window: 200K
    - [Anthropic Documentation](https://docs.anthropic.com/claude/docs/models-overview)
  - Type: close
  - Release Date: 2023/11/21

- **Claude 3**
  - Parameters Size: 20B, 70B, 2T (Haiku, Sonnet, Opus)?
    - [DR ALAN D. THOMPSON](https://lifearchitect.substack.com/p/the-memo-special-edition-claude-3)
  - Structure: Sparse Transformer
  - Training Data (Date): 40T tokens(~2023/8)?
    - [DR ALAN D. THOMPSON](https://lifearchitect.substack.com/p/the-memo-special-edition-claude-3)
  - Output Token: 4,096
    - [Anthropic Documentation](https://docs.anthropic.com/claude/docs/models-overview)
  - Context Window: 200K
    - [Anthropic Documentation](https://docs.anthropic.com/claude/docs/models-overview)
  - Type: close
  - Release Date: 2024/3/4

### Meta
- **Llama2**
  - Parameters Size: 7B, 13B, 70B
  - Structure: Transformer
  - Training Data (Date): 2T tokens
    - [llama blog](https://llama.meta.com/llama2/)
  - Output Token: 4,096?
    - [Hugging Face](https://huggingface.co/docs/transformers/v4.38.2/en/model_doc/llama2#transformers.LlamaModel)
  - Context Window: 4,096
    - [llama blog](https://llama.meta.com/llama2/)
  - Type: open source
    - [Hugging Face](https://huggingface.co/meta-llama)
  - Release Date: 2023/7/18

### Mistral AI
- **Mistral (Tiny)**
  - Parameters Size: 7B
  - Structure: Transformer
  - Training Data (Date): ?
  - Output Token: ?
  - Context Window: 32k
    - [Hugging Face](https://huggingface.co/amazon/MistralLite)
  - Type: open source
    - [Hugging Face](https://huggingface.co/mistralai)
  - Release Date: 2023/9/27

- **Mixtral 8x7B (Small)**
  - Parameters Size: 45B(use 12B)
  - Structure: SMoE (8 experts)
    - [Mistral news](https://mistral.ai/news/mixtral-of-experts/)
  - Training Data (Date): ?
  - Output Token: ?
  - Context Window: 32k
    - [Mistral news](chrome-extension://efaidnbmnnnibpcajpcglclefindmkaj/https://arxiv.org/pdf/2401.04088.pdf)
  - Type: open source
    - [Hugging Face](https://huggingface.co/mistralai)
  - Release Date: 2023/12/11

- **Mistral**
  - Parameters Size: Medium, Large
  - Structure: ?
  - Training Data (Date): ?
  - Output Token: ?
  - context window: 32k
    - [Mistral news](https://mistral.ai/news/mistral-large/)
  - Type: close
  - Release Date: 2024/2/26
