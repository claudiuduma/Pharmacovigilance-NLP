# Pharmacovigilance-NLP

# Pharmacovigilance NLP: Adverse Drug Reaction (ADR) Miner

## Overview
This repository contains the codebase for an academic/personal research project focused on **pharmacovigilance**. The goal of this project is to build a Natural Language Processing (NLP) pipeline capable of identifying and extracting user-reported adverse drug reactions (ADRs) from social media and medical forums, specifically focusing on side effects that may be unlisted or underreported in official clinical documentation.

## Objectives
* **Data Extraction:** Securely and respectfully gather public, anonymized patient-experience data from high-signal platforms (e.g., Reddit) using read-only API wrappers like PRAW.
* **Entity Extraction:** Utilize Named Entity Recognition (NER) via libraries like `spaCy` and `transformers` to identify specific medications and associated physiological/psychological symptoms in informal, conversational text.
* **Cross-Referencing:** Compare extracted symptom-drug pairs against ground-truth databases (such as the FDA Adverse Event Reporting System (FAERS) via the openFDA API) to flag potentially unlisted side effects.

## Tech Stack
* **Language:** Python 3.x
* **Data Collection:** PRAW (Python Reddit API Wrapper)
* **NLP Pipeline:** spaCy (Medical NER models), HuggingFace Transformers
* **External APIs:** openFDA API 

## API Compliance & Ethical Considerations
This project is strictly for **non-commercial, read-only research**. 
* **No Interaction:** The scraper will not post, comment, upvote, downvote, or interact with any users or communities.
* **Rate Limiting:** All data extraction strictly adheres to the official rate limits outlined by the Reddit Data API guidelines to ensure no strain is placed on the platform's infrastructure.
* **Anonymity:** No personally identifiable information (PII) or user account histories are stored. Text data is aggregated solely for linguistic and entity analysis.

## Disclaimer
This project is an experimental NLP tool and is **not intended to provide medical advice**, diagnose, treat, or cure any disease. All findings are for research purposes only.

## Project Status
🚧 **Phase 1:** API authorization, environment setup, and pipeline architecture drafting. (Current)
