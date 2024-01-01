<div align="center">
  <h1>Advanced Workflow GPTs <i>by Nerority</i></h1>
  <img src="https://skillicons.dev/icons?i=react,vite,ts" alt="Icons" />
  <br/>
  <a href="https://www.linkedin.com/in/devin-pellegrino-gt/"><kbd>🔵 LinkedIn</kbd></a>
  <a href="https://nerority.com"><kbd>🟢 Website</kbd></a>
</div>
<br/><br/>

*Under Active Construction*

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

# The Lineup

## Automated Infinite Visual Progression with Fine-Grain Control

**Description**: This GPT was originally built by me as a joke, however it wound up working so well, I decided to design a full-fletched GPT around this purpose. This results are nothing short of awesome. This GPT allows you to begin an infinite "progression" of a certain thing, that gradually progresses the image in a specified direction. Every response loops 5 times with DallE to complete 5 progressions. There is an extensive command and hotkey menu that is perfectly understood by the AI to allow seamless control of the progression in any way you desire. Super fun to use.

**Input**: Enter this command with the details filled out to begin the progression.

```!executeInfiniteProgression [description of base image, dimension to progress, direction, starting point, rate]```


**Workflow (Single Response)**:

- **Image Gen Loop** (DallE-3 x5)
- Operational Status and Command Menu

**Control**

```!addDimension [dimension, direction, starting point, progression rate]```

```!removeDimension [dimension]```

```!invertDirection [dimension]```

```!adjustRate [dimension, new progression rate]```

```!updateBase [context]```

<p align="center">
  <img src="https://github.com/nerority/Advanced-GPTs/assets/80237923/c4502ac9-e05f-48af-b724-050d7fbdac8c" alt="First" width="30%" height="3000">
  <img src="https://github.com/nerority/Advanced-GPTs/assets/80237923/0a8c0673-8018-497c-8c58-e35402c39c95" alt="Second" width="30%" height="3000">
  <img src="https://github.com/nerority/Advanced-GPTs/assets/80237923/fcca86b4-183f-408d-85cf-830290422196" alt="Second" width="30%" height="3000">
</p>

## Automated DALL-E Prompt Variation Testing

**Description**: This is an excellent GPT for image generation ideation and mass testing of an idea. This GPT achieves an advanced workflow leveraging multiple tools to automate mass-testing of prompt variations of an idea. Initially uses the python tool to detail 5 DallE prompts with different strategies for visualization. Generates one-by-one, runs all images through the image understanding model to grade renderings and prompt versions. Has fine-grain control for easy navigation.

**Input**: User Description of Desired Image

```!executeWorkflow [description of desired image]```

**Workflow (Single Response)**:
- Prompt Set Design (Python Tool)
- **Image Gen Loop** (DallE-3 x5)
- Image Analysis (Python Tool)
- Prompt Synthesis and Results

<p align="center">
  <img src="https://github.com/nerority/Advanced-GPTs/assets/80237923/3d8e7799-1f9a-4383-b1cb-49bf3d7bce70" width="40%" height="1500">
  <img src="https://github.com/nerority/Advanced-GPTs/assets/80237923/6deb9790-33a1-4a45-bdc9-0a806d0bb959" width="40%" height="1500">
</p>

## Automated High-Quality Document Analysis

**Description**: Getting the AI to properly understand and summarize both the holistic and granular aspects of long and/or complex documents has been a standing frustration with ChatGPT. This GPT automates an advanced workflow, that leverages RAG search and the python tool to achieve highly-detailed and valuable analysis of complex documents. This has been incredibly difficult to automate with accuracy, I am proud to have now solved this issue.

**Input**: User-Uploaded Document

Command `S` to start.

Command `P` to resume workflow from last checkpoint.

**Workflow**: 

```mermaid
graph TD
    A[Start]
    A -->|Generate ToC| B[Python Tool]
    B --> C[Analysis Loop]
    C -->|RAG Search| D[RAG & Python Tool]
    D -->|Iterative Process| C
    C --> E[Compile Data]
    E -->|Python Tool| F[Compilation Complete]
    F --> G[Save Data]
    G -->|Python Tool| H[File Saved]
    H --> I[End]

    style B fill:#f9d5e5,stroke:#333,stroke-width:2px
    style D fill:#e3eaa7,stroke:#333,stroke-width:2px
    style E fill:#f9d5e5,stroke:#333,stroke-width:2px
    style G fill:#f9d5e5,stroke:#333,stroke-width:2px
```

**Note**: This GPT has advanced resource management logic, and will create a checkpoint just before reaching the hard time-out. There is a hard time-out of ~ 8-10 minutes no matter what. Due to the complexity of this workflow, it can sometimes timeout before finishing. When this happens, simply enter "P" in the next input to re-establish the workflow where it left off.

<p align="center">
  <img src="https://github.com/nerority/Advanced-GPTs/assets/80237923/02e2d031-48ac-4b3f-b56a-fb2bf14443c3" width="450" height="1000">
  <img src="https://github.com/nerority/Advanced-GPTs/assets/80237923/cbb597cd-2ce9-4104-b1db-ece0f00421c9" width="450" height="1000">
</p>

## Automated Career Profile Analyst and Resume Tailoring for Target Positions

**Description**: This GPT automates tailored resume creation for target positions after building a user profile. It analyzes user-uploaded career documents, maps out professional trajectories, and crafts tailored resumes targeted towards specific job opportunities. This agent leverages a complex workflow integrating RAG Search, Python tooling, and Browser capabilities, orchestrated by ChatGPT's master model. It excels in understanding complex career narratives and aligning them with current market trends.

**Input**: User-uploaded career-related documents (e.g., resumes, cover letters, professional portfolios).

Command `S` to start.

**Workflow (Single Response)**: 
- Career Information Analysis (RAG Search)
- User Profile Knowledge Distillation (Python Tool)
- Career Progression Mapping (Python Tool)
- Job Market Research (Browser Tool)
- Tailored Resume Creation (Python Tool)
- Word Document Creation (Python Tool)

<p align="center">
  <img src="https://github.com/nerority/Advanced-GPTs/assets/80237923/78d062bf-4b65-45a3-ade9-b63c1e149588" width="40%" height="100%">
  <img src="https://github.com/nerority/Advanced-GPTs/assets/80237923/16bbb2fa-4117-475d-9ec7-a8b3b504eff6" width="40%" height="100%">
</p>

## Botanical Growth Cycle Visualizer

**Description**: This GPT is a specialized educational agent designed for high-quality visualizations of the growth cycle of a user selected plant species. 

**Input**: User-Specified Plant Species

```!executeWorkflow [plant species]```

**Workflow (Single Response)**
- Data Synthesis and Planning (Python Tool)
- **Image Gen Loop** (DallE-3 x6)
- Recap and Exploration

<p align="center">
  <img src="https://github.com/nerority/Advanced-GPTs/assets/80237923/e63917ed-a231-48bf-853a-5a0d0fe209d5" width="40%" height="1500">
  <img src="https://github.com/nerority/Advanced-GPTs/assets/80237923/228a4129-846c-4031-833c-ca443e9b29c3" width="40%" height="1500">
</p>

## Automated Prompt Refinement

**Description**: This GPT is designed to achieve a multi-step process for taking an unrefined input prompt into its refined form for GPT-4. The prompt is transformed into its JSON form, which is then run through numerous passes including analysis, enhancement, optimization, categorization, before being synthesized in its final form. This refinement process work excellently for complex tasks and creating consistently understood prompts. Also is a great way to convert random thoughts into well-structured prompts.

**Input**: User-Provided Prompt to Refine

```!executeWorkflow [prompt for analysis]```

**Workflow (Single Response)**
- Prompt Transformation to JSON (Python Tool)
- Prompt Analysis (Python Tool)
- Prompt Enhacement (Python Tool)
- Prompt Optimization (Python Tool)
- Prompt Categorization (Python Tool)
- Synthesis of the Final Prompt

<p align="center" style="display: flex; align-items: flex-start;">
  <img src="https://github.com/nerority/Advanced-GPTs/assets/80237923/3faf4c7e-fe9d-419b-aa32-1c012013a556" style="width: 40%; height: auto;">
  <img src="https://github.com/nerority/Advanced-GPTs/assets/80237923/4799f739-ba0b-48c5-8396-f8c09c0b256f" style="width: 40%; height: auto;">
</p>
