# Ex-5 Comparative Analysis of different types of Prompting patterns and explain with Various Test Scenarios
Test and compare how different pattern models respond to various prompts (broad or unstructured) versus basic prompts (clearer and more refined) across multiple scenarios like Zero-shot prompting -Few-shot prompting - Chain-of-Thought prompting.
# Aim
To test and compare how refining a prompt from a basic (zero-shot) structure to more refined patterns (few-shot, chain-of-thought) affects the quality, accuracy, and depth of responses from an AI model (ChatGPT) across a test scenario.
# Algorithm
The experiment is conducted by taking a single task and applying three different prompting techniques, as specified in the "Activity" section.

Base Scenario (Task): A logical reasoning problem.

1. Basic / Zero-Shot Prompt: A simple, direct question with no examples or reasoning guides. This is a "naive" prompt.

Prompt: "If 5 machines make 5 widgets in 5 minutes, how long would it take 100 machines to make 100 widgets?"

2. Few-Shot Prompt: The prompt is refined by providing two examples to guide the model's pattern recognition.

Prompt:

Example 1:

Q: 2 tailors make 2 shirts in 2 days. How long for 10 tailors to make 10 shirts?

A: 2 days.

Example 2:

Q: 3 printers print 3 books in 3 hours. How long for 20 printers to print 20 books?

A: 3 hours.

Task:

Q: If 5 machines make 5 widgets in 5 minutes, how long would it take 100 machines to make 100 widgets?

3. Chain-of-Thought (CoT) Prompt: The prompt is refined by instructing the model to show its reasoning step-by-step, which forces it to analyze the problem logically rather than defaulting to a surface-level pattern.

Prompt: "If 5 machines make 5 widgets in 5 minutes, how long would it take 100 machines to make 100 widgets? Let's think step by step to find the solution."

4. Evaluation: The responses generated from each prompt are analyzed for:

Accuracy: Is the final answer correct?

Quality & Depth: Is the reasoning (if any) sound? Does the model "understand" the problem?

# Conclusion
The experiment demonstrates that refined prompts are vastly superior for tasks involving logic and reasoning.

The Zero-Shot Prompt frequently fails. The model often falls for the "trick" and answers "100 minutes," as it follows the superficial text pattern (5-5-5 -> 100-100-100). This response has low accuracy.

The Few-Shot Prompt consistently succeeds. By seeing the examples, the model correctly identifies the underlying logical pattern (that the time per item is the constant). This response has high accuracy.

The Chain-of-Thought Prompt also consistently succeeds. By being forced to "think step by step," the model reasons: "If 5 machines make 5 widgets in 5 minutes, then 1 machine makes 1 widget in 5 minutes. Therefore, 100 machines will make 100 widgets in 5 minutes." This response has high accuracy and high depth.

# Result
The prompt for the above said problem executed successfully.
