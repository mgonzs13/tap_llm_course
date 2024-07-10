# tap_llm_course

## Table of Contents

1. [Introduction](#introduction)
2. [Exercises](#exercises)
   - [Exercise 1](#exercise-1)
   - [Exercise 2](#exercise-2)
   - [Exercise 3](#exercise-3)
   - [Exercise 4](#exercise-4)
   - [Exercise 5](#exercise-5)
   - [Exercise 6](#exercise-6)
   - [Exercise 7](#exercise-7)
3. [Acknowledgments](#acknowledgments)

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

This exercise presents a little example of using llama.cpp GGUF VLMs. A VLM is downloaded from Hugging Face and an image is downloaded from a URL to ask questions about it.

### Exercise 6

Coming soon

### Exercise 7

This final exercise presents how to download llama.cpp GGUF LLMs and VLMs from Hugging Face and deploy and prompt them inside the ROS 2 ecosystem using llama_ros, which is llama.cpp for ROS 2.

## Acknowledgments
