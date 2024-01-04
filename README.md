<div align="center">
  <h1>Advanced Workflow GPTs <i>by Nerority</i></h1>
  <img src="https://skillicons.dev/icons?i=react,vite,ts" alt="Icons" />
  <br/>
  <a href="https://www.linkedin.com/in/devin-pellegrino-gt/"><kbd>🔵 LinkedIn</kbd></a>
  <a href="https://nerority.com"><kbd>🟢 Website</kbd></a>
</div>
<br/><br/>

**1/04/24**: *Under active construction.. 12 more to be added*

*I will be preparing public versions of all GPTs for the store release next week for free. Links posted here likely this weekend.*

*Showcase of my Custom GPTs, featuring advanced workflows and operational logic.*

![Nerority](https://github.com/nerority/Advanced-GPTs/assets/80237923/e99891a8-9645-4e9b-a22c-7fca73177882)

My name is Devin. I specialize in engineering advanced generative AI workflows that leverage meta-functionality control. I have been mastering prompt engineering as a hobby for a long time now, and am able to design GPT's to do pretty much anything.

- Did you know you can perfectly control >5 minutes of AI tool chaining with >30 different tool calls in the same response, with 100% accuracy? 
- Or that you can have ChatGPT generate >10 DallE-3 Images in a single response, with perfect control?
- How about about having ChatGPT generate prompts for DallE-3 in the python tool, generate each of them one by one with DallE-3, back to the python tool for compilation and display, then to the prompt presentation and commands for next step, all in the same single response?

Yes, that has been possible to do with ChatGPT alone. The tool timeout threshold of 60 seconds, resets with each new tool call, allowing highly complex responses if you know how.

Want me to build your dream GPT? Get in touch.

**Contact**: devinpellegrino@gmail.com

**Site**: [nerority.com](https://www.nerority.com)

<div align="center">
<h1>The Lineup</h1>
</div>

## Automated Infinite Visual Progression with Fine-Grain Control

**Description**: This GPT was originally built by me as a joke project, however it wound up working so well, I decided to design a full-fletched GPT around this purpose. The results are nothing short of awesome. This GPT allows you to begin an infinite "progression" of a certain thing, that gradually progresses the image in a specified direction. Every response loops 5 times with DallE to complete 5 progressions. There is an extensive command and hotkey menu that is perfectly understood by the AI to allow seamless control of the progression in any way you desire. Super fun to use.

**Input**: Enter this command with the details filled out to begin the progression.

```!executeInfiniteProgression [description of base image, dimension to progress, direction, starting point, rate]```

**Control**

```!addDimension [dimension, direction, starting point, progression rate]```

```!removeDimension [dimension]```

```!invertDirection [dimension]```

```!adjustRate [dimension, new progression rate]```

```!updateBase [context]```

**Workflow (Single Response)**:
```mermaid
sequenceDiagram
    participant user as User
    participant ChatGPT
    participant Dalle as DallE-3

    user->>ChatGPT: User Input
    loop Image Gen Loop
        ChatGPT->>Dalle: Request Image Generation
        Dalle-->>ChatGPT: Return Generated Image
    end
    ChatGPT->>user: Operational Status
    ChatGPT->>user: Command Menu
```

<p align="center">
  <img src="https://github.com/nerority/Advanced-GPTs/assets/80237923/c4502ac9-e05f-48af-b724-050d7fbdac8c" alt="First" width="30%" height="3000">
  <img src="https://github.com/nerority/Advanced-GPTs/assets/80237923/0a8c0673-8018-497c-8c58-e35402c39c95" alt="Second" width="30%" height="3000">
  <img src="https://github.com/nerority/Advanced-GPTs/assets/80237923/fcca86b4-183f-408d-85cf-830290422196" alt="Second" width="30%" height="3000">
</p>

## Automated High-Quality Document Analysis

**Description**: Getting the AI to properly understand and summarize both the holistic and granular aspects of long and/or complex documents has been a standing frustration with ChatGPT. This GPT automates an advanced workflow, that leverages RAG search and the python tool to achieve highly-detailed and valuable analysis of complex documents. This has been incredibly difficult to automate with accuracy, I am proud to have now solved this issue.

**Input**: User-Uploaded Document

Command `S` to start.

Command `P` to resume workflow from last checkpoint.

**Workflow**: 
```mermaid
sequenceDiagram
    participant User
    participant ChatGPT
    participant RAG as RAG Search
    participant PythonTool as Python Tool

    User->>ChatGPT: Upload Document
    ChatGPT->>RAG: Initial Search
    RAG->>PythonTool: Generate ToC
    loop Analysis Loop
        PythonTool->>RAG: Section Focused Search
        RAG-->>PythonTool: Analysis of Section
    end
    PythonTool->>PythonTool: Compilation
    PythonTool->>ChatGPT: Save as File
    ChatGPT->>User: Display Download Link
```

**Note**: This GPT has advanced resource management logic, and will create a checkpoint just before reaching the hard time-out. There is a hard time-out of ~ 8-10 minutes no matter what. Due to the complexity of this workflow, it can sometimes timeout before finishing. When this happens, simply enter "P" in the next input to re-establish the workflow where it left off.

<p align="center">
  <img src="https://github.com/nerority/Advanced-GPTs/assets/80237923/02e2d031-48ac-4b3f-b56a-fb2bf14443c3" width="45%" height="800">
  <img src="https://github.com/nerority/Advanced-GPTs/assets/80237923/cbb597cd-2ce9-4104-b1db-ece0f00421c9" width="45%" height="800">
</p>

## Automated Career Profile Analyst and Resume Tailoring for Target Positions

**Description**: This GPT automates tailored resume creation for target positions after building a user profile. It analyzes user-uploaded career documents, maps out professional trajectories, and crafts tailored resumes targeted towards specific job opportunities. This agent leverages a complex workflow integrating RAG Search, Python tooling, and Browser capabilities, orchestrated by ChatGPT's master model. It excels in understanding complex career narratives and aligning them with current market trends.

**Input**: User-uploaded career-related documents (e.g., resumes, cover letters, professional portfolios).

Command `S` to start.

**Workflow (Single Response)**: 
```mermaid
sequenceDiagram
    participant User
    participant ChatGPT
    participant RAG as RAG Search
    participant PythonTool as Python Tool
    participant Browser as Browser Tool

    User->>ChatGPT: User Document Upload
    ChatGPT->>RAG: Career Information Analysis
    RAG-->>PythonTool: Analysis Results
    PythonTool->>PythonTool: User Profile Knowledge Distillation
    PythonTool->>PythonTool: Career Progression Mapping
    PythonTool->>Browser: Job Market Research
    Browser-->>PythonTool: Market Data
    PythonTool->>PythonTool: Tailored Resume Creation
    PythonTool->>PythonTool: Word Document Creation
    PythonTool->>ChatGPT: Resume Compiled
    ChatGPT->>User: Resume Presentation
```

<p align="center">
  <img src="https://github.com/nerority/Advanced-GPTs/assets/80237923/78d062bf-4b65-45a3-ade9-b63c1e149588" width="40%" height="100%">
  <img src="https://github.com/nerority/Advanced-GPTs/assets/80237923/16bbb2fa-4117-475d-9ec7-a8b3b504eff6" width="40%" height="100%">
</p>

## Market Trend Analysis and Prediction for Company X

**Description**: This GPT is designed to complete an advanced workflow that achieves a comprehensive market analysis for a user given company. First employs the browser tool to pull real-time information, which then passes through several iterations with the python tool to complete text and semantic analysis on the data. A basic predictive model is build and visualized in the first response, which can then be advanced upon with a simple hotkey in the next response. Works extremely well with user-provided data, for example apple stock prices for 2023 curtesy of kaggle.com.

**Input**: User-Specified Company

`!start [company]`

**Workflow**:

```mermaid
sequenceDiagram
    participant User
    participant ChatGPT
    participant PythonTool as Python Tool
    participant Browser

    User->>ChatGPT: Provide Company
    ChatGPT->>PythonTool: Initiate Data Analysis Loop
    loop Data Analysis Loop
        PythonTool->>Browser: Fetch Financial Reports & News Sentiments
        Browser-->>PythonTool: Provide Data
        PythonTool->>PythonTool: Perform Text and Sentiment Analysis
    end
    PythonTool->>PythonTool: Identify and Summarize Market Trends
    loop Impact Assessment Loop
        PythonTool->>PythonTool: Assess Trend Impact on Stock Prices
    end
    PythonTool->>PythonTool: Prepare Insights and Predictions
    PythonTool-->>ChatGPT: Compiled Data and Analysis
    ChatGPT->>User: Present Structured Report

```

**Note**: Results comparison between no user-provided data, and with a dataset included for Apple Stock Prices in 2023.

<p align="center">
  <img src="https://github.com/nerority/Advanced-GPTs/assets/80237923/708c2caf-e700-4ece-9a54-835ab11bbdc0" width="48%" height="600">
  <img src="https://github.com/nerority/Advanced-GPTs/assets/80237923/a881c549-1761-4b60-adf8-f5c972e26582" width="48%" height="600">
</p>

## Automated DALL-E Prompt Variation Testing

**Description**: This is an excellent GPT for image generation ideation and mass testing of an idea. This GPT achieves an advanced workflow leveraging multiple tools to automate mass-testing of prompt variations of an idea. Initially uses the python tool to detail 5 DallE prompts with different strategies for visualization. Generates one-by-one, compiles and presents for display with navigation control.

**Input**: User Description of Desired Image

```!executeWorkflow [description of desired image]```

**Workflow (Single Response)**:
```mermaid
sequenceDiagram
    participant User
    participant ChatGPT
    participant PythonTool as Python Tool
    participant DallE

    User->>ChatGPT: User Description Input
    ChatGPT->>PythonTool: Prompt Set Design
    loop Image Gen Loop x5
        PythonTool->>DallE: Request Image Generation
        DallE-->>PythonTool: Return Generated Image
    end
    PythonTool->>PythonTool: Compilation
    PythonTool->>ChatGPT: Present Results
    ChatGPT->>User: Prompt Synthesis and Results
    ChatGPT->>User: Command Menu
```

<p align="center">
  <img src="https://github.com/nerority/Advanced-GPTs/assets/80237923/3d8e7799-1f9a-4383-b1cb-49bf3d7bce70" width="48%" height="1500">
  <img src="https://github.com/nerority/Advanced-GPTs/assets/80237923/6deb9790-33a1-4a45-bdc9-0a806d0bb959" width="48%" height="1500">
</p>

## Automated Prompt Refinement

**Description**: This GPT is designed to achieve a multi-step process for taking an unrefined input prompt into its refined form for GPT-4. The prompt is transformed into its JSON form, which is then run through numerous passes including analysis, enhancement, optimization, categorization, before being synthesized in its final form. This refinement process work excellently for complex tasks and creating consistently understood prompts. Also is a great way to convert random thoughts into well-structured prompts.

**Input**: User-Provided Prompt to Refine

```!executeWorkflow [prompt for analysis]```

**Workflow (Single Response)**
```mermaid
sequenceDiagram
    participant user as User
    participant ChatGPT
    participant PythonTool as Python Tool

    user->>ChatGPT: Provide Initial Prompt
    ChatGPT->>PythonTool: Prompt Transformation to JSON
    PythonTool->>PythonTool: Prompt Analysis
    PythonTool->>PythonTool: Prompt Enhancement
    PythonTool->>PythonTool: Prompt Optimization
    PythonTool->>PythonTool: Prompt Categorization
    PythonTool-->>ChatGPT: Synthesis of the Final Prompt
    ChatGPT->>user: Deliver Final Prompt
```

<p align="center" style="display: flex; align-items: flex-start;">
  <img src="https://github.com/nerority/Advanced-GPTs/assets/80237923/3faf4c7e-fe9d-419b-aa32-1c012013a556" style="width: 40%; height: auto;">
  <img src="https://github.com/nerority/Advanced-GPTs/assets/80237923/4799f739-ba0b-48c5-8396-f8c09c0b256f" style="width: 40%; height: auto;">
</p>

## Automated Meta-Prompt Refinement

**Description**: This workflow is tailored specifically for the refinement of meta-prompts. Meta-prompts are extremely important for various tasks, and require a different strategy for refinement in comparison to regular prompts. Input prompts undergo a 7-step refinement workflow with a focus on abstraction and active contextualization. Meta-prompts work to establish “operational context” for complex tasks, and thus need to account for various aspects of a response, while intentionally leaving other aspects open-ended.

**Note**: Meta-Prompts can be understood as abstracted instructions that frame context in a way to control how the AI executes actual instructions that proceed.

**Input**: User-Provided Meta-Prompt or Instructions

**Workflow (Single Response)**
```mermaid
sequenceDiagram
    participant User
    participant ChatGPT
    participant PythonTool as Python Tool

    User->>ChatGPT: Provide Initial Prompt
    ChatGPT->>PythonTool: Initiate Refinement Loop
    loop Each Refinement Step
        PythonTool->>PythonTool: Step 1: Comprehensive Understanding
        PythonTool->>PythonTool: Step 2: Adaptive Contextualization
        PythonTool->>PythonTool: Step 3: Thorough Refinement & Expansion
        PythonTool->>PythonTool: Step 4: Intelligent Personalization
        PythonTool->>PythonTool: Step 5: Uptake of AI Innovations
        PythonTool->>PythonTool: Step 6: Optimization of Efficiency & Precision
        PythonTool->>PythonTool: Step 7: Proactive Experimentation & Enhancement
    end
    PythonTool->>ChatGPT: Synthesize Final Prompt
    ChatGPT->>User: Deliver Refined Prompt in Code Box
```

<p align="center" style="display: flex; align-items: flex-start;">
  <img src="https://github.com/nerority/Advanced-GPTs/assets/80237923/97051fef-c8c0-48c4-9665-a5952ad4c3ba" style="width: 40%; height: auto;">
  <img src="https://github.com/nerority/Advanced-GPTs/assets/80237923/160f0764-53c5-486b-bcb4-d44f15d56b3d" style="width: 40%; height: auto;">
</p>

## Botanical Growth Cycle Visualizer

**Description**: This GPT is a specialized educational agent designed for high-quality visualizations of the growth cycle of a user selected plant species. 

**Input**: User-Specified Plant Species

```!executeWorkflow [plant species]```

**Workflow (Single Response)**
```mermaid
sequenceDiagram
    participant User
    participant ChatGPT
    participant PythonTool as Python Tool
    participant DallE as DallE-3

    User->>ChatGPT: User Input
    ChatGPT->>PythonTool: Data Synthesis and Planning
    loop Image Gen Loop (x6)
        PythonTool->>DallE: Request Image Generation
        DallE-->>PythonTool: Return Generated Image
    end
    PythonTool->>ChatGPT: Compiled Images
    ChatGPT->>User: Recap and Exploration
```

<p align="center">
  <img src="https://github.com/nerority/Advanced-GPTs/assets/80237923/e63917ed-a231-48bf-853a-5a0d0fe209d5" width="40%" height="1500">
  <img src="https://github.com/nerority/Advanced-GPTs/assets/80237923/228a4129-846c-4031-833c-ca443e9b29c3" width="40%" height="1500">
</p>
