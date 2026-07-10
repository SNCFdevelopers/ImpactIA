# ImpactIA

<img width="1386" height="483" alt="ImpactIA_overview1" src="https://github.com/user-attachments/assets/5a380828-6974-41ce-9176-dbc579b62096" />

## Introduction

Impact’IA is a LLM environmental footprint calculator and a detailed methodology document, to help companies assess their IT environmental impact. It is the result of one year.man of research to gather academic work on this topic. 
It enables you, for 30 standard Gen AI models from Google, Anthopic, OpenAI and Mistral :
-	To compute GHG emissions, water usage, electricity consumption;
-	To visualize and understand the impact, from a component life cycle point of view;
-	To compare your results with 'similar models';
-	To get best practices for IT people in order to decrease environmental tootprint of Generative AI, which is a major concern.
Methodology is roughly “token based” as we compute environmental impacts and then translate them to unit token.
This tool was designed from a joint effort: SNCF Company, Resilio and Wavestone. Resilio and Wavestone have exceptionally skilled people and it was a pleasure for SNCF to drive this effort.

## What it is meant to be and NOT

We do NOT plan to make it an API based tool or library, industrialized, whatsoever.
We suggest this work to be directly used or integrated into other tools (potentially more appropriate for industrialization), like Ecologits, ClaudeCarbon, and any other free software and open source tool that help companies to drive environmental footprint the way THEY want rather than what SUPPLY CHAIN wants.

We hope that our metholodogy work will be used, criticized and will help improve assessment, considering companies are still lacking information from providers regarding AI environmental impact.

## Usage

Main tool is a standalone spreadsheet, with 4 parts:
-	README/Notice : explains the ideas, the principles
-	DATA/Données : the place to insert your inputs : to get results you need to know your LLM by its name, and be able to estimate or get the number of input tokens, and optionally output & embedding tokens.
-	RESULTS/Résultats : your figures. 
-	BEST PRACTICES/ Bonnes Pratiques : explore AI Ecodesign AI levers

<img width="605" height="85" alt="ImpactIA_results2" src="https://github.com/user-attachments/assets/107b8480-8458-49d6-9002-3ebc7bc9b45b" />

All computations assumptions are explained into our “Guide méthodologique” taht you will find under the /docs folder.
About Electricity Mix : see beleow country selector to adapt electricity mix is NOT implemented YET.

## Contributing
We are looking to the following contributions:
-	English translation: as for now, assets are only available in French. A translated guide would be an awesome addition to the work.
-	XLSX-to-ODF conversion is not within our area of expertise. However, we would be pleased to accept and share an OpenDocument-based implementation, which is more closely aligned with the core values of this work: interoperability, knowledge sharing, and sustainability
-	Ideas and help to integrate this work into others (potentially more appropriate for industrialization)
-	choosing electricity mix via a country selector : this is a first citizen parameter to compute results. We have in the calculation a default electricity mix, and this parameter is enough for our needs but this could be easily extended to cope with _any_ country hosting models. Often app front is in a different country. Regarding its emissions you could either, implement a country selector for this part OR take an average mix for your whole application.

We are not looking for : 
-	Pull request for new features

## License
This work is published under CC-BY-NC-SA  license.


