# Zara AI Stylist —> MVP Architecture

A conceptual system architecture for an AI-powered styling platform that helps users find and virtually try on Zara outfits for specific occasions.

## What is this?

An interactive architecture diagram built for a hackathon MVP. It visualises the full system design for an emotionally intelligent styling companion — from user onboarding to AI-generated virtual try-on.

## The Problem

- Scrolling through Zara's catalogue to find the right outfit for a specific event takes too long
- It's hard to know how clothes will look on *you* without trying them on in person
- Fashion terminology is a barrier for many shoppers

## The Solution

1. User describes their occasion and style preferences in plain language
2. AI understands intent, searches Zara's live catalogue semantically, and assembles coherent outfits
3. User virtually tries on selected items — seeing themselves in a generated portrait and motion clip
4. User saves the look and revisits before the event

## Architecture Overview

| Layer | Role |
|-------|------|
| **User Layer** | Onboarding, photo upload, style query, drag & drop try-on, outfit board |
| **AI / Intelligence** | NLP query understanding, semantic search, outfit assembly, try-on generation |
| **Data / API** | ITX-REST (live Zara inventory), vector store, user data, product image CDN |
| **Output / UI** | Product grid, styled portrait, motion scene clip, saved outfit board |

## Tech Stack

- **LLM** — Query understanding and outfit curation
- **Vector DB** — Semantic product search (Pinecone / pgvector)
- **ITX-REST API** — Live Zara inventory
- **Pixia** — Product imagery and virtual try-on generation
- **Image-to-Video** — 3–5 sec motion scene clip

## Delivery Milestones

- **M1** — Onboarding + photo upload flow
- **M2** — Search connected to ITX-REST API, returning live products
- **M3** — Product grid with real data + Pixia images
- **M4** — Drag & drop virtual try-on with generated output image
- **M5** — Full end-to-end demo

## Success Metrics

- Purchase conversion rate
- Time spent in try-on
- Saved outfits per user
- Revisit frequency before the event
- Confidence rating (1–5) after try-on
- Repeat event usage

## Live Demo

[View the architecture →](https://priyankak17.github.io/inditex_mvp_architecture)

## Built at

Hackathon 2026
