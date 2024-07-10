# tap_llm_course

## Table of Contents

1. [Introduction](#introduction)
2. [Exercises](#exercises)
   - [Exercise 1: Deployment of Quantized LLMs](#exercise-1)
   - [Exercise 2: Prompt Engineering with LangChain](#exercise-2)
   - [Exercise 3: QLoRA Finetune LLMs](#exercise-3)
   - [Exercise 4: RAG + Few-Shot + GBNF Grammars](#exercise-4)
   - [Exercise 5: Merging LLMs](#exercise-5)
   - [Exercise 6: Deployment of Quantized LLMs](#exercise-6)
   - [Exercise 7: Using LLMs and VLMs in ROS 2](#exercise-7)
3. [Acknowledgments](#acknowledgments)
   - [DMARCE Project](#dmarce-project)
   - [SELF-AIR Project](#self-air-project)

## Introduction

This course presents the exercises from the TAP (Tendencias en Aprendizaje Pronfundo) subject from the Master in Robotics and Artificial Intelligence. The goal of this course is to understand and get acquainted with LLMs and different techniques such as quantization, training through fintuning, QLoRA and Prompt Engineering. This way, these exercises are focused on downloading, deploying and prompting LLMs and VLMs in the robotics context.

## Exercises

The exercise folders contain a collection of exercises oriented toward learning how to use Large Language Models (LLMs) and their associated techniques. These exercises reinforce the concepts covered in the lessons focused on LLMs, finetuning, prompt engineering and LLM in robotics.

### Exercise 1

This basic exercise shows how to display a quantized LLM, specifically a llama.cpp GGUF LLM. First, the exercise focused on searching LLMs in Hugging Face and its leaderboards and arenas. Then, you have to choose a GGUF LLM and deploy it.

### Exercise 2

This exercise introduces the use of LangChain to display llama.cpp GGUF LLMs. It also provides an example of how to use quantized LLMs to perform Retrieval Augmented Generation (RAG).

### Exercise 3

This exercise provides an example of QLoRA finetuning a Phi-2 LLM using the Command Frame Representation (CFR) from the ERL Consumer Challenge. After finetning the LLM, the adapter is merged with the base Phi-2 and the resulting model is quantized using GGUF from llama.cpp.

### Exercise 4

This exercise provides an example of using prompt engineering to obtain similar results as in the case of exercise 3 which uses finetuning. In this case, Retrieval Augmented Generation (RAG) along with the GBNF grammars from llama.cpp are used. RAG is used to create a context for the LLM for the Few-Shot Prompting. Finally, the GBNF grammar will make the LLM always respond in the same format, which in this example is the Command Frame Representation (CFR) from the ERL Consumer Challenge.

### Exercise 5

Coming soon

### Exercise 6

This exercise presents a little example of using llama.cpp GGUF VLMs. A VLM is downloaded from Hugging Face and an image is downloaded from a URL to ask questions about it.

### Exercise 7

This final exercise presents how to download llama.cpp GGUF LLMs and VLMs from Hugging Face and deploy and prompt them inside the ROS 2 ecosystem using llama_ros, which is llama.cpp for ROS 2.

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
