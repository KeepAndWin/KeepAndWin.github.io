---
title: 'AICodeAssist Post'
date: 2024-09-22
permalink: /posts/2024/09/blog-post-1/
tags:
  - AI
  - IDE
  - LLM
  - Copilot
---
Recently, we've seen a surge in AI-powered coding assistants based on large language models. From the pioneering GitHub Copilot and Tabnine to the now-trending Cursor, who truly reigns supreme in the realm of code assistance? I'd like to share my recent experiences to give you an initial understanding of these tools (purely based on my personal insights).

# Copilot, Cursor, and Tongyi Lingma: Who's Your Ultimate Coding Assistant?

Recently, we've seen a surge in AI-powered coding assistants based on large language models. From the pioneering GitHub Copilot and Tabnine to the now-trending Cursor, who truly reigns supreme in the realm of code assistance? I'd like to share my recent experiences to give you an initial understanding of these tools (purely based on my personal insights).

## Tools Covered in This Article:

- GitHub Copilot
- Cursor
- Continue Extension with Local LLMs/Closed-source LLM APIs
- Tongyi Lingma

From my experience, I believe Cursor stands apart from the others mentioned:

Cursor is more akin to an AI-integrated product rather than a plugin. It's positioned on par with VSCode, similar to how Microsoft's Surface Pro 11 fully integrates Microsoft Copilot compared to earlier Surface Pro versions, or how the recently announced iPhone 16 incorporates Apple Intelligence compared to previous iPhone models. Cursor has developed an IDE based on the open-source VSCode that allows for deep, comprehensive integration of AI large language models across various functionalities.

If that sounds a bit vague, let me break down their features and differences with some examples.

## Plugin-Based AI Coding Assistants

### [GitHub Copilot](https://github.com/features/copilot):

![Copilot](https://i-blog.csdnimg.cn/direct/d244511038624178898d07f4b24bfd62.png#pic_center)

GitHub Copilot was one of the earliest tools in this field to catch public attention. Trained on high-quality code samples supported by GitHub and initially offering free use for Education accounts, it attracted a large user base. It's quite competent in code understanding and overall project architectural concepts. However, as it remains a plugin, I believe its main drawbacks are:

- **Poor Chinese language support**: While everyone can appreciate its help with Tab Auto-Complete, it struggles to achieve desired results for more complex algorithmic implementations, like stack-related algorithms, based on Chinese descriptions.
- **Lacks autonomous CodeBase understanding**: It doesn't provide content comprehension for entire code projects by default, requiring manual selection of files or specific code sections.
- **Limited grasp of actual frontend development effects and styles**: This likely relates to its training dataset. Since GitHub is a code hosting platform, the product can only learn optimal styles based on text, resulting in a weaker understanding of the correspondence between code and style.

A quick note on Tongyi Lingma: As a recently launched plugin-level product, its VSCode support currently only stands out for better Chinese language comprehension. No other notable features have been observed, and it doesn't support file uploads for understanding or copying.

### [Continue](https://www.continue.dev/) Extension:

![Continue](https://i-blog.csdnimg.cn/direct/1cf0ae2aee934f8180398f05d1815163.png#pic_center)

This extension supports users in code development assistance through methods such as:

1. Closed-source LLM API keys
2. Locally deployed LLMs via [LM Studio](https://lmstudio.ai/)
3. Locally deployed LLMs via [OLlama](https://ollama.com/)

Similar to GitHub Copilot, it supports:

- File and code snippet selection
- Chat interface based on selectable models
- Prompt-based code editing and **automatic debugging** using **selectable models**
- Tab Auto-Complete based on selectable models

It also supports CodeBase functionality and file upload with comprehension, as mentioned earlier.

However, its most noteworthy feature is that when using locally deployed LLMs for assistance, all functionalities support offline, disconnected use. Additionally, open-source LLMs support local fine-tuning, making it truly secure and genuinely available at any time.

## IDE-Based AI Coding Assistant

### [Cursor](https://www.cursor.com/):

![Cursor](https://i-blog.csdnimg.cn/direct/0adff003d847418cab695925cd155aba.png#pic_center)

Cursor has been gaining immense popularity lately. Like many others, I was initially skeptical.

"Isn't it just another coding assistant? What's so different about it? A Copilot clone? Why bother creating a separate IDE? Isn't that overkill?"

But after actually experiencing it, I must say it's quite impressive:

First, let's address why Cursor developed its own IDE. As I mentioned at the beginning, the main reason is:

- **It has already shifted code assistance from snippet-level and file-level to project-level**

Here are the most valuable points I've discovered so far:

1. **Project-level comprehensive CodeBase understanding**: Once your project folder is loaded in Cursor, you generally don't need to manually select individual files or snippets for AI assistance, as with plugin-level tools. Open the chat box, enter your description, click CodeBase, and it will comprehensively analyze your code and provide the results you want.
2. **Better language customization than GitHub Copilot**: It allows users to customize for Chinese responses during installation, and even supports minor languages.
3. **Project-level code editing**: While you're still copying and pasting code snippets based on LLM responses, Cursor already supports understanding your prompt and modifying code across different project files through its **Composer** feature.
4. **Enhanced multimodal comprehension**: Similar to the Continue plugin, Cursor also supports remote calling of various closed-source LLM APIs (but doesn't require individual configurations; a single subscription covers all, from Gemini and Claude to even OpenAI's O1). It fully leverages this capability, allowing users to upload not just files but also **images**. It can even generate code based on your provided expectations of page style images.
5. **Seamless transition for original VSCode users**: During installation, it allows original VSCode users to synchronize plugins and configuration files. Whether it's the IDE interface style or familiar plugins, Cursor enables VSCode veterans to get started with virtually no learning curve.

However, it's worth noting that due to its comprehensive understanding of project files and online usage, while harmless for small projects, it could potentially expose medium to large enterprise-level or startup projects. That said, the Business subscription does offer corresponding privacy protection.

## Conclusion:

Since all LLM responses love to include a conclusion, let's wrap this up.

In terms of pricing, Cursor's subscription is roughly twice that of GitHub Copilot. However, since it doesn't require users to separately configure API access for various mainstream closed-source LLMs and instead provides direct use, the price is justifiable. For individual independent developers and start-up level projects, the features and effects it offers are unprecedented and revolutionary. But if you're still a student, a beginner, or have certain security requirements, GitHub Copilot coupled with the Continue plugin is also a solid choice.

AI has arrived. With the release of O1 and the emergence of product-level AI tools like Cursor, AI has begun to permeate and deeply integrate with various industries, advancing towards understanding and solving large, complex problems. While IDEs are just development tools, AI's march forward will never stop. The AGI era will eventually come. When it does, how will we define ourselves? I'd love to hear your thoughts on this as well...
