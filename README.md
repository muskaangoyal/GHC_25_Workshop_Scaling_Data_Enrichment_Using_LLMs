# GHC_25_Workshop_Scaling_Data_Enrichment_Using_LLMs
This notebook contains the workshop portion for the "Scaling Data Enrichment Using LLMs" workshop hosted at GHC 25 in Chicago. To get started, download this notebook and upload it to google colab (https://colab.research.google.com/). 

## Introduction
Welcome! In this notebook, we will build a data enrichment pipeline using a real-estate dataset to convert basic numerical housing features into semantic signals (e.g., coffee access, food corridor, transit convenience, neighborhood vibe). We will then rebuild retrieval on top of those enriched signals to show how search suddenly becomes aligned with the way humans actually ask questions.

Our Goal: To demonstrate how to use a Large Language Model (LLM) to enrich data at scale.

Learning Objectives: By the end of this workshop, you will be able to:
1. Build a baseline vector retrieval system and diagnose why it fails on human questions.
2. Use prompt engineering patterns (Zero-Shot, Few-Shot, JSON Schema, CoT) to produce structured enrichment.
3. Make model selection decisions based on quality, latency, and cost tradeoffs.
4. Rebuild retrieval over enriched semantic signals and measure the improvement.

## Requisites
This workshop will reuqire access to OpenRouter, so open the site - https://openrouter.ai/settings/keys and generate a new key. Make sure to save this key because you will not be able to access it later. 

## Dataset used
We will use the King County (WA) Home Sales dataset. This dataset contains more than 20 years of residential home sales for King County, Washington (Seattle area) with columns about sale price, property size, and other home characteristics.
