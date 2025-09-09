# GermanPartiesQA: Benchmarking Commercial Large Language Models and AI Companions for Political Alignment and Sycophancy

## Overview

Large language models (LLMs) are increasingly shaping citizens' information ecosystems. Products incorporating LLMs, such as chatbots and AI Companions, are increasingly used for decision support and information retrieval, including in sensitive domains, raising concerns about hidden biases and growing potential to shape individual decisions and public opinion. 

GermanPartiesQA is a benchmark of 418 political statements from German Voting Advice Applications across 11 elections to evaluate six commercial LLMs. The dataset contains responses from major German political parties to various policy statements, providing a ground truth for assessing how AI systems align with different political positions.

## Dataset Description

The dataset contains **418 political statements** from German Voting Advice Applications across 11 elections that were presented to major German political parties. Each party responded to these statements with one of three positions:

- **Agree (1)**: The party supports the statement
- **Disagree (0)**: The party opposes the statement  
- **Neutral (2)**: The party takes a neutral position

### Political Parties Included
The dataset includes responses from six major German political parties:
- **SPD** (Social Democratic Party)
- **CDU/CSU** (Christian Democratic Union/Christian Social Union)
- **Greens** (Alliance 90/The Greens)
- **FDP** (Free Democratic Party)
- **AfD** (Alternative for Germany)
- **Left** (The Left Party)

### Data Structure
Each row in the dataset contains:
- **Statement information**: Year, county, unique ID, headline, German text, and English translation
- **Party responses**: Binary/ternary responses (0/1/2) for each political party
- **Rationales**: Detailed explanations (`_rationale` columns) from each party explaining their position

### File Format
- **File**: `GermanPartiesQA-1.csv`
- **Format**: CSV with semicolon (`;`) delimiter
- **Encoding**: UTF-8
- **Total statements**: 418

## Key Findings
Our evaluation reveals three specific findings:
1. **Factual limitations**: LLMs show limited ability to accurately generate factual party positions, particularly for centrist parties.

2. **Model-specific ideological alignment**: We identify consistent alignment patterns and degree of political steerability for each model across temperature settings and experiments.

3. **Claim of sycophancy**: While models adjust to political personas during role-play, we find this reflects *persona-based steerability* rather than the increasingly popular, yet contested concept of sycophancy.

## Versioning
GermanPartiesQA will be continuously updated with new political statements and party responses.
### Current Version: GermanPartiesQA-1
- Coverage: 11 federal and state elections (2021-2023)
- Statements: 418 political statements

## Citation
```bibtex
@article{GermanPartiesQA,
  title={GermanPartiesQA: Benchmarking Commercial Large Language Models and AI Companions for Political Alignment and Sycophancy},
  author={Batzner, Jan and Stocker, Volker and Schmid, Stefan and Kasneci, Gjergji},
  journal={Proceedings of the AAAI/ACM Conference on AI, Ethics, and Society},
  year={2025}
}
```
