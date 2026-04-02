# Amazon Bedrock Finance Agent


### Architecture Flow

<img width="695" height="609" alt="image" src="https://github.com/user-attachments/assets/209779ce-81af-4899-a325-b3da3599550d" />


### Process 

In this project, I  built a financial advisor agent using Amazon Bedrock that reads your spending data, categorizes expenses, calculates budgets, and generates visual charts, all through natural language conversation.

### Key services and concepts

Summary:

- AI agent building with Amazon Bedrock.
- Cross section context memory
- Agent persona creation 
- Code Interpreter for the agent to read and write Python code
- Importance of iteration in agents and how to improve upon outputs.

---

## Exploring Amazon Bedrock and Foundation Models

We will commence with signing into AWS account and setting the desired region. Then navigate to Amazon Bedrock and search for our model (Nova 2 Lite in this case).


![Image](http://learn.nextwork.org/sincere_amber_happy_silkie/uploads/aws-genai-bedrock-agent_w5x8n1q4)

### Understanding foundation models

A foundation model is a large AI model that is pre trained already on large datasets. These are commonly used everyday. In this project, Nova 2 Lite will be employed due to its cost effectiveness and lightweight scalability.

### Discovering Bedrock Agents

Unlike a simple chatbot that just answers questions, an agent can decide what actions to take, execute code, call APIs, and iterate on results. You give it instructions in plain English, and it figures out the steps on its own 

![Image](http://learn.nextwork.org/sincere_amber_happy_silkie/uploads/aws-genai-bedrock-agent_h4t7y1a5)

---

## Creating the AI Finance Agent

Finally...after much waiting..the man that everybody`s been tallking about

The agent. 

We will go into Bedrock and create an agent, choosing the desired model for the agent to use. We will exercise our prompt engineering skills by setting the required instructions, instructing the agent how to THINK in. At the same time, we will be enabling code interpreter, so that the agent can write and execute Python code. Once that is all completed, the agent will then be prepared, compiling all configurations to ready it for deployment. 

![Image](http://learn.nextwork.org/sincere_amber_happy_silkie/uploads/aws-genai-bedrock-agent_q4j6r2m8)

### Crafting the agent instructions

I initially provide the agent with the following instructions. We must ensure the practice of good prompt engineering techniques, as to receive more exact and desired outputs.

![Image](http://learn.nextwork.org/sincere_amber_happy_silkie/uploads/aws-genai-bedrock-agent_f2d8g4l6)

---

## Analyzing Spending Data with Code Interpreter

Our agent is finally put into action. For this process, I will use the transactions.csv file (same as on this repo). Uploading it into chat will lead to a spending summary, as well as receiving budget recommendations. We will understand how the agent thinks and then iterate on its instructions, as to improve the output further.

![Image](http://learn.nextwork.org/sincere_amber_happy_silkie/uploads/aws-genai-bedrock-agent_p4r7t9v1)

### How Code Interpreter processed the data

Code Interpreter allows the agent to run and write python code as to analyze the files attached by the user. 

---

## Iterating on Agent Instructions with Traces

The agents instructions are now enhanced to show more numerical data effectively.

![Image](http://learn.nextwork.org/sincere_amber_happy_silkie/uploads/aws-genai-bedrock-agent_q5s8u2w4)

---

## Enabling Cross-Session Agent Memory

Now comes the main part. The memory. To ensure the agent retains context, and can provide more enhanced outputs, we will enable agent memroy, allowing it to recall spending patterns, budget goals and make more efficient visual charts.

![Image](http://learn.nextwork.org/sincere_amber_happy_silkie/uploads/aws-genai-bedrock-agent_n5m3k7j1)

### Session summarization vs full history

Session summarization is the process of condensing a user's interaction or activity within a specific timeframe (a "session") into a brief, coherent overview. This helps understand user behavior, identify key actions, or extract important information from a series of events

![Image](http://learn.nextwork.org/sincere_amber_happy_silkie/uploads/aws-genai-bedrock-agent_t8h1g5f3)

### Testing cross-session recall

In this scenario, the agent recalls information on its suggestions and enhances upon it even further.

---

