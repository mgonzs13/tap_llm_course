# tap_llm_course

## Table of Contents

1. [Introduction](#introduction)
2. [Materials](#materials)
3. [Exercises](#exercises)
   - [Exercises 1: Deployment LLMs](#exercises-1)
   - [Exercises 2: Prompt Engineering](#exercises-2)
   - [Exercises 3: Fine-Tuning](#exercises-3)
   - [Exercises 4: Model Merging](#exercises-4)
   - [Exercises 5: Tool Calling](#exercises-5)
   - [Exercises 6: Deployment VLMs](#exercises-6)
   - [Exercises 7: Gradio](#exercises-7)
   - [Exercises 8: LLMs in ROS 2](#exercises-8)
   - [Exercises 9: Speech in ROS 2](#exercises-9)
   - [Exercises 10: A Chatbot for ROS 2](#exercises-10)
4. [Acknowledgments](#acknowledgments)
   - [DMARCE Project](#dmarce-project)
   - [SELF-AIR Project](#self-air-project)

## Introduction

This course provides practical exercises for the TAP (Tendencias en Aprendizaje Profundo) module, part of the Master’s in Robotics and Artificial Intelligence at the Universidad de León. The primary objective is to deepen students' understanding of Large Language Models (LLMs) and explore advanced techniques, including quantization, prompt engineering, fine-tuning, model merging, and tool calling for AI agents.

The course also covers Vision-Language Models (VLMs), user interface design for AI applications, and the integration of AI within the ROS 2 framework. Additionally, it includes the use of speech models such as Whisper, SileroVAD, and Piper, focusing on their application in robotics. The exercises emphasize hands-on experience with downloading, deploying, and prompting LLMs, VLMs, and speech models, specifically tailored to robotics use cases.

## Materials

- [Nvidia Driver 12.4](https://developer.nvidia.com/cuda-12-4-0-download-archive)

- Libraries:

  - [llama.cpp](https://github.com/ggerganov/llama.cpp)
  - [llama-cpp-python](https://github.com/abetlen/llama-cpp-python)
  - [llama_ros](https://github.com/mgonzs13/llama_ros)
  - [SileroVAD](https://github.com/snakers4/silero-vad)
  - [whisper.cpp](https://github.com/ggerganov/whisper.cpp)
  - [whisper_ros](https://github.com/mgonzs13/whisper_ros)
  - [piper](https://github.com/rhasspy/piper)
  - [piper_ros](https://github.com/mgonzs13/piper_ros)
  - [chatbot_ros](https://github.com/mgonzs13/chatbot_ros)
  - [LangChain](https://www.langchain.com/)
  - [Unsloth](https://unsloth.ai/)
  - [Gradio](https://www.gradio.app/)
  - [ROS 2 Humble](https://docs.ros.org/en/humble/Installation/Ubuntu-Install-Debs.html)

- Models:
  - [Qwen2.5-Coder-7B-Instruct](https://huggingface.co/Qwen/Qwen2.5-Coder-7B-Instruct)
  - [moondream2](https://huggingface.co/vikhyatk/moondream2)
  - [MiniCPM-V-2_6](https://huggingface.co/openbmb/MiniCPM-V-2_6)
  - [SileroVAD-ONNX](https://huggingface.co/mgonzs13/silero-vad-onnx)
  - [Whisper.cpp Models](https://huggingface.co/ggerganov/whisper.cpp)
  - [Piper Models](https://huggingface.co/rhasspy/piper-voices)

## Exercises

The exercise folders contain a collection of exercises oriented toward learning how to use Large Language Models (LLMs) and their associated techniques. These exercises reinforce the concepts covered in the lessons focused on LLMs, Fine-Tuning, Prompt Engineering, Model Merging, Tool Calling, and LLM in robotics.

### Exercises 1

These basic exercises show how to deploy a quantized LLM, specifically a [llama.cpp](https://github.com/ggerganov/llama.cpp) GGUF LLM, using [llama-cpp-python](https://github.com/abetlen/llama-cpp-python). First, the exercise focused on searching LLMs in Hugging Face and its leaderboards and arenas. Then, you have to choose a GGUF LLM and deploy it. Finally, compare the use of a chat version of an LLM with the vanilla version.

### Exercises 2

These exercises introduce Prompt Engineering by using [LangChain](https://www.langchain.com/). Therefore, [LangChain](https://www.langchain.com/) is used to deploy [llama.cpp](https://github.com/ggerganov/llama.cpp) GGUF LLMs. It also provides examples of how to use quantized LLMs to perform Retrieval Augmented Generation (RAG), with Embedding models and Reranker models. Finally, a Structured Output example is included using GBNF grammars from [llama.cpp](https://github.com/ggerganov/llama.cpp).

### Exercises 3

These exercises provide examples of Fine-Tuning, PEFT (Parameter-Efficient Fine-Tuning), and QLoRA, using [Unsloth](https://unsloth.ai/). Specifically, there are two PEFT types employed: SFTT (Supervised Fine-tuning Trainer), used to train an LLM to generate Behaviour Trees (Dataset: [ArtemLykov/LLM_BRAIn_dataset](https://huggingface.co/datasets/ArtemLykov/LLM_BRAIn_dataset)), and DPO (Direct Preference Optimization), used to focus an LLM on neural networks data (Dataset: [NeuralNovel/Neural-DPO](https://huggingface.co/datasets/NeuralNovel/Neural-DPO)). After Fine-Tuning the LLMs, the LoRA adapters can be merged with the base LLMs and quantize the resulting LLM or quantize the LoRA adapters.

### Exercises 4

These exercises provide examples of Model Merging to create new LLMs instead of using Fine-Tuning. There are two types of merging in these exercises: SLERP (Spherical Linear Interpolation), used to merge a Qwen model and a DeekSeek model, and Passthrough, used to merge several Qwen models. The resulting LLMs are quantized to GGUF.

### Exercises 5

This exercise presents a basic use of Tool Calling, using AI Agents. Since [llama-cpp-python](https://github.com/abetlen/llama-cpp-python) only supports calling a function, this basic example shows how an LLM can be used to create a tool call.

### Exercises 6

These exercises present a basic example of using a VLM through [llama-cpp-python](https://github.com/abetlen/llama-cpp-python). The VLM is downloaded from Hugging Face and an image is downloaded from a URL to ask questions about it.

### Exercises 7

These exercises present a basic example of using a [Gradio](https://www.gradio.app/) to create a web chatbot. An LLM is deployed using [llama.cpp](https://github.com/ggerganov/llama.cpp). Then, the chatbot history is used to prompt the model. The resulting responses are shown in the web interface.

### Exercises 8

These exercises present how to download [llama.cpp](https://github.com/ggerganov/llama.cpp) GGUF LLMs and VLMs from Hugging Face and deploy and prompt them inside the ROS 2 ecosystem using [llama_ros](https://github.com/mgonzs13/llama_ros), which is [llama.cpp](https://github.com/ggerganov/llama.cpp) for ROS 2.

### Exercises 9

These exercises present Speech example for ROS 2. First of all, it shows how to download [whisper.cpp](https://github.com/ggerganov/whisper.cpp) and [SileroVAD](https://github.com/snakers4/silero-vad) models, from Hugging Face, to perform Automatic Speech Recognition (ASR) in ROS 2 ecosystem using [whisper_ros](https://github.com/mgonzs13/whisper_ros), which is [whisper.cpp](https://github.com/ggerganov/whisper.cpp) for ROS 2. Additionally, these exercises present a TTS (Text-to-Speech) example using [piper](https://github.com/rhasspy/piper) through [piper_ros](https://github.com/mgonzs13/piper_ros).

### Exercises 10

These exercises present how to deploy a full chatbot in ROS 2 ([chatbot_ros](https://github.com/mgonzs13/chatbot_ros)). The chatbot will use [whisper_ros](https://github.com/mgonzs13/whisper_ros) to perform the Automatic Speech Recognition (ASR), [llama_ros](https://github.com/mgonzs13/llama_ros) to produce responses, and [piper_ros](https://github.com/mgonzs13/piper_ros) to speak the responses.

## Acknowledgments

### DMARCE Project

Decision Making in Autonomous Robots: Cybersecurity and Explainability (DMARCE).

DMARCE (EDMAR+CASCAR) Project: EDMAR PID2021-126592OB-C21 -- CASCAR PID2021-126592OB-C22 funded by MCIN/AEI/10.13039/501100011033 and by ERDF A way of making Europe

<p align="center">
    <img src="https://user-images.githubusercontent.com/3810011/192087445-9aa45366-1fec-41f5-a7c9-fa612901ecd9.png" width="49%" /> <img src="https://raw.githubusercontent.com/DMARCE-PROJECT/DMARCE-PROJECT.github.io/main/logos/micin-uefeder-aei.png" width="46%" />
</p>

### SELF-AIR Project

Supporting Extensive Livestock Farming with the use of Autonomous Intelligent Robots

Grant TED2021-132356B-I00 funded by MCIN/AEI/10.13039/501100011033 and by the “European Union NextGenerationEU/PRTR"

<p align="center">
    <img src="https://raw.githubusercontent.com/shepherd-robot/.github/main/profile/robotics_wolf_minimal.png" width="13.5%" /> <img src="https://raw.githubusercontent.com/shepherd-robot/.github/main/profile/micin-financiadoUEnextgeneration-prtr-aei.png" width="60%" />
</p>
