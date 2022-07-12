# 📝 Text Corpus
Contributors and collaborators help to develop text corpus from original and new sources that are licensed under creative commons zero (CC0). 

You can use a variety of methods such as; 

* [sentence collector](https://commonvoice.mozilla.org/sentence-collector/#/how-to) to contribute CC0 licensed content 
* [bulk submission]() to contribute large files of sentences in txt format 
* [sentence extractor](https://github.com/Common-Voice/cv-sentence-extractor) from large sources of public domain text, with a focus easy-to-read corpus and Wikipedia.

⚠️ _ Mozilla Common Voice datasets are released under a CC0 “No Rights Reserved” License and are part of the public domain. This means that works subject to copyright cannot be added to Common Voice datasets. But some copyright owners are willing to make a [CC0 waiver](https://common-voice.github.io/community-playbook/sub_pages/cc0waiver_process.html), dedicating their work to the public domain so that it can be contributed to Common Voice.

## Why is Sentence collection Important?
Currently, Common Voice requires voice donations to be tied to sentences, by sourcing more sentences people are able to donate more hours of voice data. Sentence Collection Bands](https://discourse.mozilla.org/t/share-your-views-nuancing-sentence-collection-requirements-new-sentence-collection-bands/93134) were introduced to support the entry-level for the voice collection stage.
* 5,000 sentences     _allow_     5,5 hrs of voice
* 9,000 sentences     _allow_     10 hrs of voice
* 90,000 sentences    _allow_     100 hrs of voice
* 1,800,000 sentences _allow_     2000 hrs of voice

## What should I consider when contributing Sentences?
It’s also important to ensure sentences are readable to speakers across all backgrounds. 

### Sentence Diversity 
Phoneome, variant and domain diversity are crucial in ensuring that the dataset can understand the vastness of language. All sentences in the dataset can be viewed on the [Common Voice Github](https://github.com/common-voice/common-voice/tree/main/server/data). If you notice a gap regarding sources or types of content, we encourage you to add more sentences to help diversify the text corpus

For example, some languages have Gramaitical Gender e.g Abogado and Abogada mean Male Lawyer and Female Lawyer respectively Spanish. 
⚠️ _ As part of the [Common Voice 2022 Product Roadmap](https://docs.google.com/spreadsheets/d/137YOs41kbzXyai6_Kn_lu08EHAziPt4ioPUkuSFSSTc/edit?usp=sharing) we are scoping and delivering a domain-specific text corpus on the platform 

### Community Participation Guidelines (CPG)
It’s important that everyone and every language can have enjoyable experiences in contributing to Common Voice. Sentences that include harmful content or violations of the CPG, will be reviewed and subsequently deleted. 

### Skills Needed 

**Sentence extraction**
🔨 _Skills required to help: Command line usage and git, familiar with regular expressions._

**Sentence collection**
🔨 _Skills required to help: Strong grammar knowledge of the target language you are contributing to._

**Large corpus validation**
🔨 _Skills required to help: Expertise in processing and cleaning up text, linguistics/language expertise to check the quality of the resulting sentences._

## Tooling development

Contributors also develop, maintain and update the sentence extractor and collector code.
* Sentence Extractor: 🐞 [Open issues](https://github.com/Common-Voice/cv-sentence-extractor/projects/1?fullscreen=true) - 🔨 _Skills needed: Rust_
* Sentence Collector: 🐞 [Open issues](https://github.com/Common-Voice/sentence-collector/projects/2?fullscreen=true) - 🔨 _Skills needed: React, JavaScript, Node.js_
