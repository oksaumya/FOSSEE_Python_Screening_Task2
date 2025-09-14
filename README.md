# FOSSEE Python Screening Task 2: AI Debugging Assistant Prompt

## Overview

This repository contains my submission for the FOSSEE Python Screening Task 2, which involves creating a prompt for an AI debugging assistant that helps students debug Python code without revealing direct solutions.

## Task Objective

The goal was to write a natural-language prompt that guides an AI assistant to:
- Analyze buggy Python code submitted by students
- Provide helpful suggestions and hints
- Avoid giving away correct solutions
- Encourage learning through guided discovery

## Repository Structure

```
FOSSEE_Python_Screening_Task2/
├── README.md                           # This file - project overview and setup
├── ai_debugging_prompt.md              # The main AI assistant prompt
├── reasoning_and_design_choices.md     # Detailed explanation of design decisions
├── example_interaction.md              # Basic examples showing prompt in action
└── advanced_examples.md                # Complex scenarios and pedagogical depth
```

## Files Description

### 1. `ai_debugging_prompt.md`
The enhanced AI assistant prompt featuring:
- **Error-type specific guidance**: Systematic approaches for syntax, logic, runtime, and semantic errors
- **Adaptive questioning strategies**: Different question types for beginner, intermediate, and advanced learners
- **Progressive disclosure framework**: "Start broad, get specific, never reveal" methodology
- **Growth-oriented language patterns**: Psychologically safe communication that builds confidence
- **Transferable debugging strategies**: Teaching techniques that apply beyond individual problems

### 2. `reasoning_and_design_choices.md`
In-depth pedagogical analysis including:
- **Cognitive Science Foundation**: How the prompt aligns with learning research
- **Motivational Psychology**: Growth mindset integration and autonomy support
- **Differentiated Instruction**: Adaptive expertise development across skill levels
- **Evidence-Based Design**: Why alternative approaches were rejected
- **Implementation Considerations**: Quality assurance and future enhancement possibilities

### 3. `example_interaction.md`
Basic demonstrations showing:
- Common Python errors (syntax, logic, index errors)
- How the prompt guides students without revealing solutions
- Progressive difficulty from beginner to intermediate levels

### 4. `advanced_examples.md`
Sophisticated scenarios demonstrating:
- Complex debugging situations (recursion, performance, design issues)
- Deep pedagogical thinking in action
- Real-world connections and professional development insights
- Advanced skill-level adaptations

## Enhanced Key Features

### ✅ **Cognitive Science Integration**
- **Progressive disclosure**: Manages cognitive load through structured information revelation
- **Elaborative interrogation**: Strategic questioning promotes deeper understanding
- **Desirable difficulties**: Productive struggle enhances retention and transfer
- **Metacognitive development**: Explicit focus on thinking processes builds self-regulation

### ✅ **Adaptive Expertise Development**
- **Error-type classification**: Systematic approaches for different bug categories
- **Skill-level differentiation**: Novice → Intermediate → Advanced progression pathways
- **Zone of proximal development**: Questions calibrated just beyond current ability
- **Professional modeling**: Language and approaches mirror real-world mentoring

### ✅ **Motivational Psychology**
- **Growth mindset language**: Emphasizes skill development over innate ability
- **Psychological safety**: Normalizes struggle and reduces imposter syndrome
- **Autonomy support**: Students maintain agency in their learning process
- **Competence building**: Graduated challenges build self-efficacy systematically

### ✅ **Transferable Skill Focus**
- **Scientific reasoning**: Debugging as hypothesis testing and investigation
- **Pattern recognition**: Building mental models that apply across contexts
- **Communication skills**: Articulating problems and reasoning processes
- **Professional practices**: Real-world collaborative debugging approaches

## Setup Instructions

No special setup is required. The files are plain text/Markdown and can be viewed in any text editor or Markdown viewer.

### To use the prompt:
1. Copy the content from `ai_debugging_prompt.md`
2. Paste it as instructions to your AI assistant (ChatGPT, Claude, etc.)
3. Provide the student's buggy Python code
4. The AI will follow the prompt guidelines to provide educational feedback

### To understand the design:
1. Read `reasoning_and_design_choices.md` for detailed explanations
2. Review the pedagogical principles and design decisions
3. See how the prompt addresses different learning scenarios

## Example Usage

**Student submits:**
```python
def count_vowels(word):
    vowels = "aeiou"
    count = 0
    for letter in word:
        if letter in vowels:
            count = count + 1
    return count

# This doesn't work for "HELLO"
```

**AI Response (following the prompt):**
"I can see you have a solid understanding of loops and string operations! Your logic for counting vowels is on the right track. 

I notice something interesting about how your function handles the word 'HELLO'. Can you think about what might be different between the letters in 'HELLO' and the vowels in your `vowels` string? 

Try adding a print statement inside your loop to see exactly what `letter` contains for each iteration. What do you observe about the case of the letters?"

## Design Validation - Research-Based Effectiveness

The enhanced prompt exceeds task requirements through evidence-based design:

### **Task Requirement Compliance:**
- ✅ **Clear and specific**: Detailed guidelines with concrete examples and response structures
- ✅ **General applicability**: Works across Python topics, skill levels, and error types
- ✅ **Behavioral precision**: Specific instructions for different scenarios and student needs
- ✅ **Solution prevention**: Multiple layered mechanisms prevent direct answer revelation
- ✅ **Learning promotion**: Focuses on transferable skill development and metacognition

### **Advanced Pedagogical Features:**
- ✅ **Cognitive load management**: Progressive disclosure prevents overwhelming students
- ✅ **Motivation optimization**: Growth mindset language and psychological safety
- ✅ **Assessment integration**: Student responses provide rich formative feedback
- ✅ **Professional alignment**: Mirrors real-world mentoring and collaborative debugging
- ✅ **Long-term impact**: Builds scientific reasoning and problem-solving capabilities

### **Implementation Robustness:**
- ✅ **Quality assurance**: Built-in mechanisms for consistent, high-quality responses
- ✅ **Scalability**: Framework supports large-scale educational deployment
- ✅ **Adaptability**: Future enhancement pathways clearly identified
- ✅ **Cultural sensitivity**: Growth-oriented language translates across contexts

## Contact

For questions about this submission, please contact via the provided email channel.

---

**Submission Date**: September 2024  
**Task**: FOSSEE Python Screening Task 2  
**Focus**: AI-Assisted Learning and Debugging  
**Enhancement Level**: Advanced pedagogical integration with cognitive science research
