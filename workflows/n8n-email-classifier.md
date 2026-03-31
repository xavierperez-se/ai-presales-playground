# AI Email Classification Workflow (n8n + Ollama)

## Overview
This workflow classifies incoming emails using a local LLM.

## Objective
Reduce manual triage and test a practical AI automation use case.

## Categories
- phishing
- spam
- newsletter
- other

## Workflow logic
1. Fetch email from IMAP
2. Extract subject and body
3. Send content to Ollama
4. Parse the output:
   - category
   - confidence
5. Apply rules:
   - if confidence is high enough, classify automatically
   - otherwise default to "other"

## Why it matters
This experiment combines:
- automation
- local AI inference
- structured decision logic

## Stack
- n8n
- Ollama
- local LLM
- IMAP
