# Advanced Workflow GPTs

*Showcase of my custom GPTs, featuring advanced workflows and operational context. These are some of the best GPTs in the world.*

My name is Devin. I specialize in engineering advanced AI workflows that leverage meta-functionality control. I have been mastering prompt engineering for almost 2 years now as a hobby, but I am now able to get GPT's to do pretty much anything.

- Did you know you can perfectly control >5 minutes of AI tool chaining with >30 different tool calls in the same response, with 100% accuracy? 
- Did you know you can have ChatGPT generate >10 Dalle Images in a single response, with perfect control?
- Did you know you can have ChatGPT generate prompts for DallE in the python tool, generate each of them one by one with DallE, pull them into the image understanding model to accurately critique the generated images, and then determine the best prompt, all in the same single response?

Yes, that has been possible to do with just ChatGPT. The timeout window of 60 seconds, resets with each new tool call, allowing highly complex responses if you know how.

# Introducing the GPTs

## Automated High-Quality Document Analysis

**Description**: Getting the AI to properly understand and summarize both the holistic and granular aspects of long and/or complex documents has been a standing frustration with ChatGPT. This GPT automates an advanced workflow, that leverages RAG search and the python tool to complete highly detailed and valuable analysis of complex documents. This has been incredibly difficult to automate with accuracy, I am proud to have solved this issue.

**Input**: Uploaded Document

**Workflow**: 
- Generate ToC (Python Tool)
- **Analysis Loop** (RAG Search & Python Tool)
- Compilation (Python Tool)
- Save as File (Python Tool)

**Note**: There is a hard time-out of ~ 8-10 minutes no matter what. Due to the complexity of this workflow, it can sometimes timeout before finishing. When this happens, simply enter "P" in the next input to re-establish the workflow where it left off.

## Automated Career Profile Analyst and Resume Tailoring for Target Positions

**Description**: This GPT automates tailored resume creation for target positions after building a user profile. It meticulously analyzes user-uploaded career documents, maps out professional trajectories, and crafts tailored resumes targeted towards specific job opportunities. This GPT leverages a sophisticated workflow integrating RAG Search, Python tooling, and Browser capabilities, orchestrated by ChatGPT's master model. It excels in understanding complex career narratives and aligning them with current market trends.

**Input**: User-uploaded career-related documents (e.g., resumes, cover letters, professional portfolios).

**Workflow (Single Response)**: 
- Career Information Analysis (RAG Search)
- User Profile Knowledge Distillation (Python Tool)
- Career Progression Mapping (Python Tool)
- Job Market Research (Browser Tool)
- Tailored Resume Creation (Python Tool)
- Word Document Creation (Python Tool)

## Automated DALL-E Prompt Refinement with Fine-Grain Control

**Description**: This is an excellent GPT for image generation. This GPT completes an advanced workflow leveraging multiple tools to automate approach to a "perfect" prompt. Has fine-grain control for easy navigation.

**Input**: User Description of Desired Image

**Workflow (Single Response)**:
- Prompt Set Design (Python Tool)
- **Image Gen Loop** (DallE-3 x5)
- Image Analysis (Python)
- Prompt Synthesis and Results

## Automated Infinite Visual Progression with Explicit Control

**Description**: This GPT was originally build by me as a joke, however it wound up working so well, I decided to make a full fletched GPT built around this purpose. This results are nothing short of amazing. This GPT allows you to begin an infinite "progression" of a certain thing, that gradually progresses the image in a specified direction. Every response loops 5 times with DallE to complete 5 progressions. There is an extensive command and hotkey menu that is perfectly understood by the AI to allow seamless control of the progression in any way you desire. Super fun to use.

**Input**: Enter this command with the details filled out to begin the progression.

```!executeInfiniteProgression [description of base image, dimension to progress, direction, starting point, rate]```

**Workflow (Single Response)**:
- **Image Gen Loop** (DallE-3 x5)

## Botanical Growth Cycle Visualizer

**Description**: This GPT is a specialized educational agent designed for high-quality visualizations of the growth cycle of a user selected plant species. 

**Input**: User Specified Plant Species

**Workflow**:
- Data Synthesis and Planning (Python Tool)
- **Image Gen Loop** (DallE-3 x6)
- Recap and Exploration

## Hyper-Dimensional Scientific Theory Synthesizer

**Description**: This is a GPT specifically designed to synthesize novel scientific theories that are grounded in empirical evidence. This is more of an experiment at this point, but still very cool nonetheless.

**Input**: User specified subfield for theory-crafting or uploaded document with theory details to advance upon.

**Workflow (Single Response)**:
- Reflective Analysis of Existing Theories (Browser Tool)
- Results Detailing (Python Tool)
- Synthesis of New Theory (Python Tool)
- Empirical Grounding (Python Tool)
- Innovative Insight Integration (Python Tool)
- Alightment Check for Empirical Grounding (Browser Tool)
- Final Results and Command Menu

## Perfected Prompt Template AI Program

**Description**: This is specialized GPT intended to streamline conversation management with long and complex generative AI chats. It is designed to parse conversational context with in depth understanding, and design high-quality prompts that are designed to improve upon the process detailed in the conversation.

**Input**: Uploaded document with conversation details

**Workflow**:
- Initial Understanding (RAG)
- Logic Synthesis and Refinement (Python Tool)
- Recursive Learning and Iterative Improvement (Python Tool)(Optional Loop)
- Prompt Validation and Adjustment (Python Tool)
- Prompt Presentation
