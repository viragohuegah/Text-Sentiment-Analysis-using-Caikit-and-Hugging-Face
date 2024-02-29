# Text Sentiment Analysis using Caikit and Hugging Face

## Table of Contents
1. [Overview](#overview)
2. [Mentee Info](#mentee-info)
3. [Technologies Used](#technologies-used)
4. [Setup](#setup)
5. [Usage](#usage)
7. [Structure](#structure)
8. [Project Status](#project-status)

<a name="overview"></a>
## Overview
<br>Mentee assignment from IBM Advance AI @ Infinite Learning Course completion of Text Sentiment Analysis using Caikit and Hugging Face from [CognitiveClass.ai](https://cognitiveclass.ai/courses/course-v1:IBMSkillsNetwork+GPXX0PYAEN+v1)

We will build a Python application that uses Caikit run-time and API to query the Hugging Face model for sentiment analysis on text strings.

<a name="mentee-info"></a>
## Mentee Info
| Nama             | Program              |
| ---------------- | -------------------- |
| Rizqi Hairunnisa | IBM Advance AI 🤖🌊 |



<a name="technologies-used"></a>
## Technologies Used

- numpy - version 1.21.3



<a name="setup"></a>
## Setup
You can setup your project by cloning this repository and install the libraries above.

For specific version of the libraries, please check the `requirements.txt` file. You can install the libraries by using the command below.

```bash
pip install -r requirements.txt
```

<a name="usage"></a>

## Usage
You can run the program by using the command below.

```bash
python client.py
```


<a name="structure"></a>
## Structure
```bash
├── text-sentiment/                     # top-level package directory
│   ├── README.md
│   ├── start_runtime.py                # a wrapper to start the Caikit runtime as a gRPC server. The runtime will load the model at startup
│   ├── client.py                       # client which calls the Caikit runtime to perform inference on the model it is serving to perform text sentiment analysis
│   ├── requirements.txt                # specifies library dependencies
│   ├── models/                         # a directory that contains the Caikit metadata of the model and any artifacts required to run the model
│   │   ├── text_sentiment/config.yml   # metadata that defines the Caikit text sentiment model
│   ├── text_sentiment/                 # a directory that defines Caikit module(s) that can include algorithm(s) implementation that can train/run an AI model
│   │   ├── config.yml                  # configuration for the module and model input and output
│   │   ├── __init__.py                 # makes the data_model and runtime_model packages visible
│   │   ├── data_model/                 # a directory that contains the data format of the Caikit module
│   │   │   ├── classification.py       # data class that represents the AI model attributes in code
│   │   │   ├── __init__.py             # makes the data model class visible in the project
│   │   ├── runtime_model/              # a directory that contains the Caikit module of the model
│   │   │   ├── hf_module.py            # a class that bootstraps the AI model in Caikit so it can be served and used (infer/train)
└── └── └── └── __init__.py             # makes the module class visible in the project


```

<a name="project-status"></a>

## Project Status
Project is: _complete_

