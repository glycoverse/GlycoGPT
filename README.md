# GlycoGPT

[![Static Badge](https://img.shields.io/badge/gpt-store-blue?logo=openai&labelColor=black&color=white)](https://chatgpt.com/g/g-692979f3c97481919a1aae952c8f7d77-glycogpt)
[![name status badge](https://glycoverse.r-universe.dev/badges/:name)](https://glycoverse.r-universe.dev/)

<p align="center">
  <img width="375" height="159" alt="glycoverse-chatgpt" src="https://github.com/user-attachments/assets/3030c58e-37e0-4790-81ae-a999b21494f1" />
</p>

<p align="center">
  <span style="background: linear-gradient(45deg, #12c2e9, #c471ed, #f64f59); -webkit-background-clip: text; -webkit-text-fill-color: transparent;">
    <strong>Your GPT assistant for glycoverse<br>Powered by <a href="https://chatgpt.com/">ChatGPT</a></strong>
  </span>
</p>

---
GlycoGPT is an AI-powered bioinformatics assistant specialized in glycomics and glycoproteomics data analysis.
Built on top of the glycoverse ecosystem, GlycoGPT is designed to help researchers streamline workflows, understand package functionalities, and generate analysis-ready code with best practices in mind.

<p align="center">
  <img width="588" height="405" alt="截屏2025-11-28 22 11 34" src="https://github.com/user-attachments/assets/5e397d44-83ff-424f-b283-5c1db8aaba45" />
</p>

GlycoGPT understands all full glycoverse packages, including:

- [glyexp](https://github.com/glycoverse/glyexp) — data management
- [glyread](https://github.com/glycoverse/glyread) — data import and cleaning
- [glyclean](https://github.com/glycoverse/glyclean) — data preprocessing
- [glystats](https://github.com/glycoverse/glystats) — statistical analysis
- [glyvis](https://github.com/glycoverse/glyvis) — visualization
- [glyrepr](https://github.com/glycoverse/glyrepr) — glycan representation
- [glyparse](https://github.com/glycoverse/glyparse) — structure parsing
- [glymotif](https://github.com/glycoverse/glymotif) — motif analysis
- [glydet](https://github.com/glycoverse/glydet) — derived trait analysis
- [glyenzy](https://github.com/glycoverse/glyenzy) — biosynthesis pathway analysis
- [glydb](https://github.com/glycoverse/glydb) — glycan databases
- [glyanno](https://github.com/glycoverse/glyanno) — annotation and information enhancement

As a domain-aware assistant, GlycoGPT aims to:

- Provide accurate, reproducible R code using glycoverse functions
- Encourage best practices in glycoverse-based data analysis
- Offer guidance on workflows, interpretation, and visualization
- Help both beginners and advanced users explore the glycoverse ecosystem

---
## How to Use?

Click [![Static Badge](https://img.shields.io/badge/gpt-store-blue?logo=openai&labelColor=black&color=white)](https://chatgpt.com/g/g-692979f3c97481919a1aae952c8f7d77-glycogpt) and start chatting!

>[!Note]
>GlycoGPT requires 5.1-thinking for best results. Other models might give incorrect codes.

## Common Usages

> I have a StrucGP result file. How do I get glycosites with at least one core-fucosylated glycans?

> How do I create a `glyexp::experiment()` object?

> Give me the vignette about IUPAC-condensed glycan structure strings.

> I have some compositions. I want to know all possible structures in batch.

> Explain the `glyclean::auto_clean()` function to me.

> Can I calculate derived traits for glycoproteomics data?

Always provide more details if you can. For example:

> I have a pGlyco3 result file with glycan structures. I also have sample information stored in a CSV file. The file contains two columns: "sample" for sample names, and "group" for disease group. "group" can be either "cancer" or "healthy". How I can get glycosites with unregulated core-fucosylation level in cancer samples?

## Other Models?

If you are using LLMs other than ChatGPT, copy and paste the prompt below should work.

>[!Note]
>Please use latest models with thinking and web access for best results, such as gemini-3-pro or claude-opus-4.5.

```
# Instruction

Now you're a bioinformatics expert in glycomics and glycoproteomics. Your job is to help users get familiar with the glycoverse. Please do the following things in order:

1. Visit the resources below to get a basic understanding of glycoverse.
2. Using what you just learned, complete the following task.
3. If you encounter anything not sure about glycoverse, visit the documentation or even the source code again.

# Introduction of glycoverse

The ‘glycoverse’ is a set of packages that together form a comprehensive pipeline for glycomics and glycoproteomics data analysis.

This includes:

- glyexp: for data management
- glyread: for data import
- glyclean: for data cleaning and preprocessing
- glystats: for statistical analysis
- glyvis: for data visualization
- glyrepr: for glycan structure representation
- glyparse: for glycan structure parsing
- glymotif: for glycan structure motif analysis
- glydet: for glycan derived trait analysis
- glyenzy: for glycan biosynthesis pathway analysis
- glydb: for glycan structures in database
- glyanno: for glycan information enhancement

# Resources

- Source code: https://github.com/glycoverse/[PACKAGE]
- r-universe: https://glycoverse.r-universe.dev/

Read the Get Started with xxx vignette for the package you want to use:

https://glycoverse.r-universe.dev/articles/[PACKAGE]/[PACKAGE].html

You might need to get the documentation of each function by:

https://glycoverse.r-universe.dev/[PACKAGE]/doc/manual.html#[FUNCTION]

# Coding style

- Assume that the user has installed all glycoverse packages, including the meta-package glycoverse.
- Omit argument passing if what you pass in is the same as the default values.
- Before using any glycoverse function, please refer to the documentation to check all arguments and return values.
- Before using any other packages, think twice if the functionality is provided in glycoverse.
- Please also load `tidyverse` using `library(tidyverse)`.
- When calling a function in glycoverse, use `f()` directly. `pkg::f()` is not good.
```
