# 🛠️ Step 3: Selecting the LLM Model

## Model Options

### OpenAI LLMs:
- **Pros:** Strong function calling, multimodal capabilities, and robust performance.
- **Cons:** Higher cost compared to some other models.

### Claude LLMs:
- **Pros:** Excellent for storytelling and conversational tasks.
- **Cons:** May not be as versatile for technical tasks.

### Open-source LLMs (e.g., Llama 3, Mixtral 8x7B, Falcon, etc.)
- **Pros:** More control over training data and compute. Cheaper inferencing cost.
- **Cons:** Limited abilities and reliability. 

---

## Configure Model in Code
Example: Set `model="gpt-3.5-turbo"` in API calls.

### Design System Prompt
- Include instructions for the **Thought/Action/Observation** loop.
- Define available actions and their usage.
- Provide example interaction.

```python
system_prompt = """
You are an AI assistant capable of performing actions and reasoning about your responses.
Follow this format for your thoughts and actions:
Thought: Reason about the task and decide on the next action.
Action: <action_name>: <action_input>
Observation: The result of the action will be provided here.

Available actions:
1. wikipedia(query): Search Wikipedia for information.
2. calculate(expression): Evaluate mathematical expressions.
3. simon_blog_search(query): Search Simon's blog for relevant posts.

Example interaction:
Human: What's the capital of France and what's its population plus 1000?
AI: To answer this question, I'll need to perform two actions.
Thought: First, I need to find the capital of France.
Action: wikipedia: capital of France
Observation: Wikipedia result for 'capital of France': https://en.wikipedia.org/wiki/Paris
Thought: Now that I know the capital is Paris, I need to find its population and add 1000.
Action: wikipedia: population of Paris
Observation: Wikipedia result for 'population of Paris': https://en.wikipedia.org/wiki/Paris
Thought: The population of Paris is approximately 2,140,526 (as of 2019). Now I need to add 1000 to this number.
Action: calculate: 2140526 + 1000
Observation: Result of '2140526 + 1000': 2141526
"""
```

---

## Considerations

### Performance Metrics
Evaluate models based on their performance metrics (e.g., accuracy, latency).

### Cost Efficiency
Consider the cost associated with each model and its fit within your budget.

### Feature Set
Ensure the model supports the features required for your specific use case.

---

## Next Steps
- Experiment with different models to compare their efficiency.
- Implement logging and monitoring for better performance tracking.
- Optimize model usage based on real-world needs and constraints.

## Contributing
Feel free to contribute by submitting issues or pull requests!

## License
[MIT License](LICENSE)
