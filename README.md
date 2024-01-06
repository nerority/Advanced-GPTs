<div align="center">
  <h1>Advanced Workflow GPTs <i>by Nerority</i></h1>
  <img src="https://skillicons.dev/icons?i=react,vite,ts" alt="Icons" />
  <br/>
  <a href="https://www.linkedin.com/in/devin-pellegrino-gt/"><kbd>🔵 LinkedIn</kbd></a>
  <a href="https://nerority.com"><kbd>🟢 Website</kbd></a>
</div>
<br/><br/>

*Showcase of my Custom GPTs, featuring advanced workflows and operational logic.*

*I will be preparing public versions of all GPTs for the store release next week for free. This page will see constant updates over the weekend and links will be live by Monday (1/08/24).*

<details>
  <summary><b>Under active construction... (click to view changelog)</b></summary>
  
  ## Changelog
  - Update 1: 3 New GPTs: Automated Knowledge Distillation, Business Contract Analyzer, Advanced Competitive Analysis AI. Pending SS
  - Update 2: First 3 GPTs workflows massively updated and refined for public use. Final Testing.
  <!-- Add more updates here -->
</details>

---

![Nerority](https://github.com/nerority/Advanced-GPTs/assets/80237923/e99891a8-9645-4e9b-a22c-7fca73177882)

Hi my name is Devin. I specialize in engineering advanced generative AI workflows that leverage meta-functionality control. I have been mastering prompt engineering as a hobby for a long time now, and am able to design GPT's to do pretty much anything.

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

### Quick Nav
1. [Automated Infinite Visual Progression with Fine-Grain Control](#automated-infinite-visual-progression-with-fine-grain-control)
2. [Automated Career Profile Builder, Resume Optimizer, and Target Position Tailoring](#automated-career-profile-builder-resume-optimizer-and-target-position-tailoring)
3. [Automated High-Quality Document Analysis](#automated-high-quality-document-analysis)
4. [Automated Market Trend Analysis and Prediction for Target Company](#automated-market-trend-analysis-and-prediction-for-target-company)
5. [Automated DALL-E Prompt Variation Testing](#automated-dall-e-prompt-variation-testing)
6. [Automated Prompt Refinement](#automated-prompt-refinement)
7. [Automated Meta-Prompt Refinement](#automated-meta-prompt-refinement)
8. [Botanical Growth Cycle Visualizer](#botanical-growth-cycle-visualizer)
9. [Automated Knowledge Distillation](#automated-knowledge-distillation)
10. [Business Contract Analyzer](#business-contract-analyzer)
11. [Advanced Competitive Analysis AI](#advanced-competitive-analysis-ai)

</br>

---

## Automated Infinite Visual Progression with Fine-Grain Control

**Status**: Finalized for Release

### Description

This GPT was originally built by me as a joke project, however it wound up working so well, I decided to design a full-fletched GPT around this purpose. The results are nothing short of awesome. This GPT allows you to begin an infinite "progression" of a certain thing, that gradually progresses the image in a specified direction. Every response loops 5 times with DallE to complete 5 progressions. There is an extensive command and hotkey menu that is perfectly understood by the AI to allow seamless control of the progression in any way you desire. Super fun to use.

### User Commands

**Input**:

- `!executeIP[description of base image, dimension to progress, direction, starting point, rate]`
- `!demo` - Executes the workflow for ai synthesized data to demonstrate and test the workflow
- `!commands` - Displays the command menu for the user

**Control**

- `!addDimension [dimension, direction, starting point, progression rate]`
- `!removeDimension [dimension]`
- `!invertDirection [dimension]`
- `!adjustRate [dimension, new progression rate]`
- `!updateBase [context]`
- `N` - Proceed with the next set of 5 progressions.

## Workflow (Single Response):
```mermaid
sequenceDiagram
    participant User
    participant ChatGPT
    participant DallE as DALL-E

    User->>ChatGPT: Inputs Commands (e.g., !executeIP)
    ChatGPT->>DallE: Initial Image Generation
    DallE-->>ChatGPT: Initial Image
    loop Progressive Visualization Loops
        ChatGPT->>DallE: Progress Image in Specified Dimensions
        DallE-->>ChatGPT: Progressed Image
    end
    ChatGPT-->>ChatGPT: Compile Progression Status
    ChatGPT->>User: Displays Current Progression Status Menu
    ChatGPT->>User: Presents User Command Menu
    User->>ChatGPT: Inputs Next Commands (e.g., N, O, E)
    Note over ChatGPT: Resource Management and Continuation Setup
```

<p align="center">
  <img src="https://github.com/nerority/Advanced-GPTs/assets/80237923/c4502ac9-e05f-48af-b724-050d7fbdac8c" alt="First" width="30%" height="3000">
  <img src="https://github.com/nerority/Advanced-GPTs/assets/80237923/0a8c0673-8018-497c-8c58-e35402c39c95" alt="Second" width="30%" height="3000">
  <img src="https://github.com/nerority/Advanced-GPTs/assets/80237923/fcca86b4-183f-408d-85cf-830290422196" alt="Second" width="30%" height="3000">
</p>

---

## Automated Career Profile Builder, Resume Optimizer, and Target Position Tailoring

**Status**: Finalized for Release

### Description

I went a little too hard on this one but the end result is pretty amazing. This GPT is designed to execute an extremely complex workflow that automates the full process of user profile building in a multi-step process with strategic RAG searches, into browser searches for real-time job market information, and finally creating an optimized, high-fidelity, tailored general-purpose resume aligned with current market trends. All simply from an uploaded document of career-related context. I have added a pause to the workflow for many reasons after testing for public release. Saving the profile first allows seamless follow-up and full resources dedicated to resume crafting. The profile saved in the first step is the "distilled knowledge" of your career profile. You can save it, edit or refine it, and use it in many different ways for AI-driven applications as a base knowledge source. Next update I will be adding logic to accept distilled profiles from the start, to execute a more advanced workflow.

After the first phase is complete, you should enter `C` and allow the workflow to finish the 2nd phase. After the final resume is saved, you can use the next steps for automated quality tailoring for any position. Simply feed the description in and the comprehensive context is pre-framed for high-quality tailoring.

I know full well how annoying applying for jobs can be for the average person in the current day. With the level of expected tailoring and ATS systems to deal with, it is a full-time job and more on its own. This was intended from the start to shake things up once and for all. Make me proud 😎

### User Commands

- `!start` - Initiates the advanced workflow based on the uploaded document
- `!demo` - Demonstrate the workflow for user with AI synthesized data
- `P` - Resume the workflow from the last saved checkpoint
- `G` - Synthesize the refined resume with markdown formatting.
- `J` - Complete a new tailored resume based on user provided job description or search

### Workflow

```mermaid
sequenceDiagram
    participant User
    participant ChatGPT
    participant PythonTool as Python Tool
    participant RAG as RAG Search
    participant Browser as Browser Tool

    note over User, ChatGPT: Phase 1
    User->>ChatGPT: Uploads Career Documents
    ChatGPT->>RAG: Initial Comprehensive Profile Analysis
    RAG-->>PythonTool: Extracted Career Information
    PythonTool->>PythonTool: High-Level Profile Knowledge Distillation
    PythonTool-->>ChatGPT: High-Level Profile
    ChatGPT->>RAG: Detailed Experience Analysis
    RAG-->>PythonTool: Search Results
    PythonTool->>PythonTool: Detailed Experience Mapping
    PythonTool-->>ChatGPT: Updated Profile
    ChatGPT->>RAG: Comprehensive Skills Analysis
    RAG-->>PythonTool: Search Results
    PythonTool->>PythonTool: Detailed Skill Mapping
    PythonTool-->>ChatGPT: Updated Profile
    PythonTool->>PythonTool: Final Profile Synthesis, Save File
    PythonTool->>ChatGPT: Save Link
    ChatGPT->>User: Present Link and Commands
    note over User, ChatGPT: Pause

    note over User, ChatGPT: Phase 2
    User->>ChatGPT: Continue (C)
    ChatGPT->>Browser: Job Market Research
    Browser-->>PythonTool: Job Listings and Requirements
    PythonTool->>PythonTool: Synthesize Search Findings and Strategize
    PythonTool-->>ChatGPT: Findings and Strategy
    ChatGPT->>PythonTool: Manually Write the Full Tailored Resume
    PythonTool->>PythonTool: Save and Format Tailored Text
    PythonTool-->>ChatGPT: Save File 
    ChatGPT->>User: Display Resume Link, Hotkeys for Navigation
```

<p align="center">
  <img src="https://github.com/nerority/Advanced-GPTs/assets/80237923/af8554ef-091f-41e3-9abc-2a1659c37efb" width="60%" height="100%">
</p>

---

## Automated High-Quality Document Analysis

**Status**: Finalized for Release

### Description

Getting the AI to properly understand and summarize both the holistic and granular aspects of long and/or complex documents has been a standing frustration with ChatGPT. This GPT automates an advanced workflow, that leverages strategic RAG searches and the python tool to achieve highly-detailed and valuable analysis of complex documents. This has been incredibly difficult to automate with accuracy, I am proud to have now solved this issue.

### Intended Usage

Complex documents that have coherent structure. This GPT will generate a TOC based on a first pass, and then start an analysis loop with seperate searches for every section sequentually. This is a long-horizon process, and can take multiple full response timeouts to complete depending on the complexity of the information and the ToC structure. For more strategic searching or faster processes, there are more specialized GPTs for that later in this portfolio.

**Input**: User-Uploaded Document

### User Commands

- `!start` - Initiates workflow based on user uploaded document.
- **`C` -** Re-establish the workflow where it left off.
- **`R` -** Restart the analysis with a new document.
- **`E` -** End the current analysis session.

### Planned Improvements

- Adding final pass to save in different formats without breaking fidelity
- Expanding out command set and post-actions

### Workflow

```mermaid
sequenceDiagram
    participant User
    participant ChatGPT
    participant RAG as RAG Search
    participant PythonTool as Python Tool

    User->>ChatGPT: Uploads Document
    ChatGPT->>RAG: Initial Document Analysis
    RAG-->>PythonTool: Holistic Understanding of Content
    PythonTool->>PythonTool: Create TOC Skeleton in JSON
    PythonTool->>ChatGPT: Display TOC
    loop Detailed Section Analysis
        ChatGPT->>RAG: Analyze Specific Section
        RAG-->>PythonTool: Section Insights
        PythonTool->>PythonTool: Synthesize Insights into TOC
    end
    PythonTool->>PythonTool: Compile Final Report
    PythonTool->>ChatGPT: Save and Provide Report Link
    ChatGPT->>User: Offer User Commands (C, R, E)
```

**Note**: This GPT has advanced resource management logic, and will create a checkpoint just before reaching the hard time-out. There is a hard time-out of ~ 6-8 minutes no matter what. Due to the complexity of this workflow, it will often timeout before finishing. When this happens, simply enter "C" in the next input to re-establish the workflow where it left off. After a recent update by OpenAI, this timeout can sometimes "freeze" the screen with an error, just refresh the page, and even if the prior analysis windows disappeared, just use C and it will pick up where it left off until complete.

<p align="center">
  <img src="https://github.com/nerority/Advanced-GPTs/assets/80237923/02e2d031-48ac-4b3f-b56a-fb2bf14443c3" width="45%" height="800">
  <img src="https://github.com/nerority/Advanced-GPTs/assets/80237923/cbb597cd-2ce9-4104-b1db-ece0f00421c9" width="45%" height="800">
</p>

---

## Automated Market Trend Analysis and Prediction for Target Company

**Status**: Testing and Refinement for Public Use

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

---

## Automated DALL-E Prompt Variation Testing

**Status**: Testing and Refinement for Public Use

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

---

## Automated Prompt Refinement

**Status**: Testing and Refinement for Public Use

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

---

## Automated Meta-Prompt Refinement

**Status**: Testing and Refinement for Public Use

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

---

## Botanical Growth Cycle Visualizer

**Status**: Testing and Refinement for Public Use

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

---

# Under Construction

*Need to design a GPT for Automated Testing and Screens xD*

## Automated Knowledge Distillation

**Status**: Initial Testing Done, Pending Refinement for Public Release

**Description**: This GPT is a powerful tool for anyone looking to quickly extract meaningful information from dense and lengthy documents. It reduces the time and effort required to parse through complex materials, providing clear, concise summaries of essential content. This tool is particularly valuable in academic research, business intelligence, legal analysis, and any other field where the rapid assimilation of detailed information is crucial.

**Input**: User uploads a document for analysis.

**Commands**:

- `!start` to initiate the document upload and analysis.
- `!refine [keywords]` for focused extraction on specific topics or concepts.

**Workflow**:

```mermaid
sequenceDiagram
    participant User
    participant ChatGPT
    participant RAG as RAG Search
    participant PythonTool as Python Tool

    User->>ChatGPT: Uploads Document
    ChatGPT->>RAG: Initial Full Document Search
    RAG-->>PythonTool: Document Understanding
    PythonTool->>PythonTool: Create Strategy for Knowledge Distillation
    PythonTool-->>ChatGPT: Knowledge Distillation Strategy
    loop RAG Search Loop for Key Concepts
        ChatGPT->>RAG: Execute Focused Searches
        RAG-->>PythonTool: Search Results on Key Concepts
        PythonTool->>PythonTool: Synthesize Results in JSON
    end
    PythonTool->>ChatGPT: Compile and Synthesize Knowledge Summary
    ChatGPT->>User: Present Knowledge Summary in Code Box
```

**Screenshots**: *Placeholder*

## Business Contract Analyzer

**Status**: Initial Testing Done, Pending Refinement for Public Release

**Description**: This advanced workflow leverages the full capabilities of RAG Search for detailed content extraction and the Python tool for strategic planning and data synthesis, ensuring a thorough analysis of legal contracts. The process is designed to be efficient and comprehensive, catering to the needs of legal professionals who require in-depth contract analysis.

**Input**: User-uploaded Legal Document for Strategic Analysis

- `!start` to initiate the document upload and analysis.

### Sequence Diagram

```mermaid
sequenceDiagram
    participant User
    participant ChatGPT
    participant RAG as RAG Search
    participant PythonTool as Python Tool

    User->>ChatGPT: Uploads Document
    ChatGPT->>RAG: Initial Full Document Search
    RAG-->>ChatGPT: Document Understanding
    ChatGPT->>PythonTool: Create Strategy for Deeper Searches
    PythonTool-->>ChatGPT: Deeper Search Strategy
    loop RAG Search Loop x3
        ChatGPT->>RAG: Execute Deeper Search (Analyze Contract, Key Clauses, Risk Assessment)
        RAG-->>PythonTool: Search Results
        PythonTool->>PythonTool: Synthesize Results in JSON
    end
    PythonTool->>ChatGPT: Compile and Synthesize Analysis Report
    ChatGPT->>User: Present Analysis Report
```

**Screenshots**: *Placeholder*

## Advanced Competitive Analysis AI

**Status**: Initial Testing Done, Pending Refinement for Public Release

**Description**: In the realm of business, understanding the competitive landscape is crucial for strategic decision-making. This GPT is specifically tailored for quality real-time competitive analysis of a user defined scope. It serves as an essential tool for comprehensively understanding industry dynamics, competitive positioning, and emerging market trends. By leveraging the combined power of ChatGPT, Python, and the Browser tool, this workflow delivers deep insights into competitors’ strategies and market movements, enabling users to make informed decisions and stay ahead in their respective industries.

**Input**: Users begin by providing key details such as their industry, main competitors, and specific areas of interest.

Commands:

- `!startAnalysis [industry] [competitors] [interest areas]` to initiate the analysis.
- `!refineReport` to refine the report based on user feedback.

**Workflow**:

```mermaid
sequenceDiagram
    participant User
    participant ChatGPT
    participant PythonTool as Python Tool
    participant Browser

    User->>ChatGPT: Provide Industry, Key Competitors, Areas of Interest
    ChatGPT->>PythonTool: Plan Data Collection Queries and Prepare for Loop
    PythonTool-->>ChatGPT: Search Queries and Plan
    loop Data Collection and Analysis Loop (For each planned search)
        ChatGPT->>Browser: Search Competitors and Market Trends
        Browser-->>PythonTool: Gathered Data
        PythonTool->>PythonTool: Process and Analyze Data
    end
    PythonTool->>PythonTool: Identify Patterns and Strategic Insights
    PythonTool->>PythonTool: Generate Report and Recommendations
    PythonTool-->>ChatGPT: Compiled Report
    ChatGPT->>User: Present Final Report in Code Box
    loop User Feedback Loop
        User->>ChatGPT: Provide Feedback
        ChatGPT->>PythonTool: Refine Report Based on Feedback
    end

```

**Screenshots**: *Placeholder*
