# AI Language Models Overview

## Introduction
Welcome to this comprehensive overview of the current landscape of AI language models. This document is designed to be a living resource that captures the specifications and release details of various large-scale language models developed by leading technology companies.

The aim is to provide a centralized, up-to-date comparison of these models, which range from OpenAI's GPT series to Google's offerings and beyond. For researchers, developers, and enthusiasts, this comparison serves as a quick reference to understand the capabilities, structures, and unique features of each model.

## Language Models
In this section, we delve into each company's contributions to the field of AI language models. We outline the models they have released, specifying parameters such as model size, underlying structures, training data, token output capacity, context window, type (whether open source or closed source), and release dates.

Understanding these details is crucial for anyone interested in the technical aspects of AI development or looking to leverage these models for various applications.

## Contributions
The world of AI is ever-evolving, and keeping this document up to date is a community effort. Whether you have corrections, updates, or new information, your contributions are invaluable to ensure the accuracy and completeness of this resource.

Please feel free to submit pull requests with your updates or open an issue if you have questions or suggestions for improvement. Let's collaborate to make this a definitive resource for everyone interested in the progress of AI language models!

We welcome and appreciate contributions from all members of the AI and tech community.

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
    - [Link](https://community.openai.com/t/how-many-parameters-does-gpt-3-5-have/648417/4)
  - Structure: Transformer
  - Training Data (Date): 45T (~2021/09)
    - [Link](https://community.openai.com/t/what-is-the-size-of-the-training-set-for-gpt-3/360896)
  - Output Token: 4,096
  - context window: 4k~16k
  - Type: close
  - Release Date: 2022/3/15

- **GPT-4**
  - Parameters Size: 8*220B (Plus, Team, Enterprise)
    - [Link](#)
  - Structure: MoE (8 experts)
  - Training Data (Date): ?
    - [Link](#)
  - Output Token: 4,096
  - context window: 32k (Plus, Team) 128K(Enterprise)
  - Type: close
  - Release Date: 2023/4/4

### Google
- **PaLM 2**
  - Parameters Size: 340B (Unicorn, Bison, Otter, Gecko)
    - [Link](#)
  - Structure: Transformer
  - Training Data (Date): 3.6T (~2023/8)
    - [Link](#)
  - Output Token: 1024~8192
  - context window: 8K~32K
  - Type: close
  - Release Date: 2023/5/10

- **Gemma**
  - Parameters Size: 2B, 7B
    - [Link](#)
  - Structure: Transformer
  - Training Data (Date): 2T, 6T tokens
    - [Link](#)
  - Output Token: ?
  - context window: 8K
  - Type: open source
  - Release Date: 2024/2/21

- **Gemini 1.0**
  - Parameters Size: Nano1(1.8B), Nano2(3.3B), Pro, Ultra
    - [Link](#)
  - Structure: Transformer
  - Training Data (Date): ?
    - [Link](#)
  - Output Token: 2,048
  - context window: 8K
  - Type: close
  - Release Date: 2024/2/8

- **Gemini 1.5**
  - Parameters Size: Pro
    - [Link](#)
  - Structure: MoE
  - Training Data (Date): ?
    - [Link](#)
  - Output Token: 8,192
  - context window: 128k~1m
  - Type: close
  - Release Date: 2024/2/15

### Anthropic
- **Claude 2.1**
  - Parameters Size: 200B
    - [Link](#)
  - Structure: Evolved Transformer
  - Training Data (Date): ? (~Early, 2023)
    - [Link](#)
  - Output Token: 4,096
  - context window: 200K
  - Type: close
  - Release Date: 2023/11/21

- **Claude 3**
  - Parameters Size: 20B, 70B, 2T (Haiku, Sonnet, Opus)
    - [Link](#)
  - Structure: Sparse Transformer
  - Training Data (Date): 40T tokens(~2023/8)
    - [Link](#)
  - Output Token: 4,096
  - context window: 200K
  - Type: close
  - Release Date: 2024/3/4

### Meta
- **Llama2**
  - Parameters Size: 7B, 13B, 70B
    - [Link](#)
  - Structure: Transformer
  - Training Data (Date): 2T tokens
    - [Link](#)
  - Output Token: 4096
  - context window: 4,096
  - Type: open source
  - Release Date: 2023/7/18

### Mistral AI
- **Mistral (Tiny)**
  - Parameters Size: 7B
    - [Link](#)
  - Structure: Transformer
  - Training Data (Date): ?
    - [Link](#)
  - Output Token: ?
  - context window: 32k
  - Type: open source
  - Release Date: 2023/9/27

- **Mixtral 8x7B (Small)**
  - Parameters Size: 45B(use 12B)
    - [Link](#)
  - Structure: SMoE (8 experts)
  - Training Data (Date): ?
    - [Link](#)
  - Output Token: ?
  - context window: 32k
  - Type: open source
  - Release Date: 2023/12/11

- **Mistral**
  - Parameters Size: Medium, Large
    - [Link](#)
  - Structure: ?
  - Training Data (Date): ?
    - [Link](#)
  - Output Token: ?
  - context window: 32k
  - Type: close
  - Release Date: 2024/2/26
