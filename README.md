# AI-powered-Parenting-Assistant

## Overview: 
The Parenting AI Assistant is designed to provide real-time, AI-powered guidance to parents who need advice on handling various parenting situations. The assistant processes both text and audio inputs, allowing parents to either describe their parenting concerns through text or speak them out via voice recordings. By leveraging Natural Language Processing (NLP) techniques and predefined agents, the assistant delivers respectful, insightful, and practical parenting advice.

This project aims to guide parents through their challenges by offering:
- Practical parenting strategies based on input data.
- Emotional analysis of the parent's tone or wording.
- Parenting tips from a knowledge base.

## Key Features:
1. 	**Input Options:**
    - Text Input: Parents can type out their concerns or situations.
    - Audio Input: Parents can record their concerns, and the system will convert the audio to text using speech-to-text models.
2.	**Parenting Advice:**
    - The core functionality of the AI Assistant is to analyze the parent's input and provide practical and respectful parenting advice based on predefined NLP models.
    - The advice is generated through a Recommendation Agent, which pulls information from an extensive knowledge base on respectful parenting principles.
3.	**Emotional Analysis:**
    - The system evaluates the emotional tone of the parent's input using sentiment analysis techniques.
    - An Emotion Detection Agent identifies stress, frustration, or calmness in the parent's tone, allowing for tailored advice based on their emotional state.
4.	**Parenting Tips:**
    - The assistant provides actionable parenting tips and strategies from the Knowledge Management Agent, which draws on a library of parenting techniques, tips, and resources.
    - The tips focus on practical ways to handle the child's behavior and improve parent-child relationships.
5.	**Relevance Check:**
    - The assistant checks whether the input is related to parenting issues. If the input is not parenting-related, the system informs the user that it can only provide parenting assistance, ensuring that the advice remains relevant.
6.	**Multi-Agent System:**
    - The AI Assistant uses a combination of agents, each specializing in a specific function (Recommendation, Emotion Detection, Knowledge Management), to provide well-rounded advice.
7.	**Gradio Interface:**
    - A user-friendly Gradio interface is integrated into the notebook, allowing parents to interact with the AI Assistant easily.
    - Users can either type their concerns or record them, with results displayed in a clear, organized format.
8.	**Speech-to-Text:**
    - The assistant can process voice recordings by converting them into text using a speech recognition system. This is especially useful for parents who prefer speaking rather than typing.

## Technical Components

- **Libraries:** CrewAI, Langchain, Transformers, Numpy, Gradio
- **APIs:** Cohere
- **Web Framework:** Gardio

## Workflow
**User Input:**

- The parent provides input through the Gradio interface, either by typing their parenting concern or recording their voice. The voice input is transcribed into text using the Whisper ASR model.

**Relevance Detection:**

- The system checks whether the input is related to parenting using keyword matching or NLP classification. If the input is not relevant to parenting, the assistant responds with a message stating that it only provides parenting-related advice.

**Emotion Analysis:**

- The Emotion Detection Agent analyzes the emotional tone of the input to determine if the parent is stressed, frustrated, or calm. This step ensures that the assistant can provide emotionally supportive responses tailored to the parent's current state of mind.

**Parenting Advice Generation:**

- The Recommendation Agent uses pre-trained NLP models fine-tuned for parenting to generate personalized, respectful, and context-specific advice based on the parent's input. The advice is rooted in established parenting principles and techniques.

**Parenting Tips and Resources:**

- The Knowledge Management Agent provides additional tips, strategies, and resources. This could include behavior management techniques, communication strategies, or links to relevant parenting resources.
  
**Final Output Aggregation:**

- The Final Output Agent combines the advice from the Recommendation Agent, emotional analysis from the Emotion Detection Agent, and tips from the Knowledge Management Agent into a cohesive response.
- This output includes practical advice, emotional validation, and actionable parenting tips, all tailored to the specific issue presented by the user.

**Output:**

- The curated response is presented back to the parent through the Gradio interface, providing them with actionable parenting advice, emotional support, and helpful resources, all in real-time.

