# MCQ Creator using Large Language Models (LLM)

A Jupyter notebook-based pipeline that uses advanced language models like OpenAI's GPT models to generate Multiple Choice Questions (MCQs) from a given PDF input.

## Problem Statement

Traditionally, creating multiple choice questions from textual content is time-consuming, prone to biases, and can sometimes lack the desired variety or depth. The aim of this project is to automate this process while maintaining high-quality standards for the generated MCQs.

## Usecase

This tool can be especially useful for:
* Educators looking to generate quiz questions from textual content.
* Content creators aiming to engage their audience with interactive quizzes.
* E-learning platforms in need of generating a multitude of questions from educational materials.

## Features

1. **Advanced LLM Integration:** Utilizes powerful language models for generating MCQs.
2. **Structured Output:** Ensures standardized MCQ format for easy integration.
3. **Extraction Mechanism:** Retrieves MCQs from markdown code blocks in the generated output.

## Project Workflow

1. **MCQ Creation Pipeline:**
   * Retrieve the most relevant answer to a given question from the LLM.
   * Utilizes different "chain types" like "map_reduce", "refine", and "map-rerank" to improve the quality of the answer retrieval.

2. **Output Structuring:**
   * Define the desired MCQ structure: question, available choices, and correct answer.
   * Initialize a ChatGPT model for MCQ generation.

3. **Prompt Formatting:**
   * Create a guiding prompt template for the ChatGPT model.
   * Include specific formatting instructions for the desired structured output.

4. **MCQ Extraction:**
   * Extract MCQs using regex operations from the markdown text, capturing all generated MCQs.

## Potential Improvements

* More robust regex patterns to handle complex JSON structures.
* Implementing a feedback loop to improve MCQ quality.
* Redundancy checks to ensure diverse question generation.
* Specifying MCQ difficulty levels.

