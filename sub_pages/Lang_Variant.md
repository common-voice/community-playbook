# Community guidance for languages and variants

## Background

We want to support communities in deciding what [variants](https://foundation.mozilla.org/en/blog/how-we-are-making-common-voice-even-more-linguistically-inclusive/) are required for their languages and how best to organise and structure their language within the Common Voice platform. This guidance will be in the form of a set of questions and descriptions.

A general guide is that the more people who are included in a single dataset, the better the dataset will be. We want machines to be able to understand how young and old people speak, how people with different gender identities speak and how mother-tongue speakers and learners speak. The more voices we include, the more inclusive we are, the better and more reliable systems trained on the data will be.

## Definitions 

Here are some definitions to be thinking about when you determine how your language should be represented in Common Voice.


| Name   |      Definition   |  
|----------|:-------------:|
| Language (or linguistic system) |  A language is tricky to define, broadly speaking it defines a group of speakers who can understand each other (‘mutual intelligibility’). It has to do with history and society as well as with linguistics. | 
| Written Language |   Languages can be written in different ways that may be closer or further from how they are spoken.  Written language does not just faithfully reproduce something that someone has said, but can also have rules of its own. Different communities may speak in the same way, but have different rules for how their language is written.| 
| Variant (or dialect) | No two people speak exactly the same, everyone has their own way of speaking. Some ways of speaking are more similar to each other than to others. When multiple speakers identify themselves with a particular way of speaking (in terms of vocabulary and grammatical rules) we call this a variant. This identification can be based on many factors, but the most common of which is region. These differences may be visible in the written language or they may not.| 
| Accent | When people use the same vocabulary and grammar but pronounce words differently then we call this an accent, a speaker may have more than one accent in a language. Accent is not a variation from a standard (all speakers have an accent), but rather variation within a linguistic system.| 


## General approach 

### Subtitle: Understanding the changes 

#### Using  ISO-639-3 to inform your decision about whether you need your own language code?

The International Standards Organisation (ISO) has developed a standardised way of referring to languages. This standard is called ISO-639-3 and provides each language with a separate alphabetic code.

There are two main sets of language codes currently widely used, one set uses two letters and one set uses three letters. For example, the two-letter code for English is en but the three-letter code is eng.

In many cases languages that had one two letter code have several three letter codes, for example ku “Kurdish” has three letter variants kmr “Northern Kurdish” and ckb “Central Kurdish”. If the language has a separate three letter code then it is likely to constitute a separate language for the purposes of Common Voice. Although this choice is up to the language community, for example Western Armenian has a separate three-letter code hyw, but the Armenian community has chosen to stay together in a single language under the hy code.

You can check the list of language codes at the following Wikipedia link:
https://en.wikipedia.org/wiki/List_of_ISO_639-3_codes

### What if some  countries, communities and regions have very different vocabulary?

In many cases languages as spoken in different places have different words for the same thing, for example in English what is called a lorry [eng-GB] in England might be called a truck [eng-US] in the United States. Similarly, in Mexico, the word for computer is computadora [spa-MX], while in Spain it is ordenador [spa-ES]. 

It might also be that there are differences within a country, such as between regions or between urban and rural areas. For example, Catalan spoken in the Valencian area has different words and different endings on verbs, such as eixir “to go out” [cat-valencia] versus sortir “to go out” [cat].

When people have exposure to many different varieties they are often familiar with the differences, but will only use the one that applies to their own. If there are large and well defined differences then it can be worth representing with different variants in Common Voice. 

### Are words in the language pronounced differently in different countries or regions?

If the language is mostly written the same way, but words are pronounced differently in different countries or regions or communities then you may want to represent this using accents. This includes if there are regular differences in writing. For example, spelling differences between US and non-US English, the word colour [eng] may be spelt color, but the difference in spelling doesn’t change how the word is pronounced. 

Sometimes there may be a lot of major differences in spelling and pronunciation, such as dreamt [eng] in the United Kingdom versus dreamed in the United States, or huit [cat] “eight” in the west of the Catalan-speaking area versus vuit [cat] “eight” in the east. This may call for a different variant.

### Do some speakers use a different writing system to write the language?

Some languages are written with different writing systems depending on where they are spoken. For example Serbian can be written in Cyrillic, река “river” [srp-Cyrl] and Latin reka “river” [srp-Latn]. Other examples would be Konkani (Latin and Devanagari), Punjabi (Perso-Arabic and Devanagari) or Crimean Tatar (Latin and Cyrillic). For the moment these can be best treated as variants, but multiple orthographies for the same language or variant will be possible later in 2022.

When people use the same vocabulary and grammar but pronounce words differently then we call this an accent, a speaker may have more than one accent in a language. 

Accent is not a variation from a standard (all speakers have an accent), but rather variation within a linguistic system.

### Do some countries, regions or groups write words very differently?

In some places the same writing system is used, but words are written very differently but there are differences in how words are written (or spelt). For example Basaa is a language of Cameroon, it can be written in multiple ways, one way is older and another way is newer. For example the word “father” would be ǹsaŋ in the new orthography [bas-academy] but nsañ in the older one [bas-mission] but not everyone wants to use the new system or is familiar with it. In this case, the two different ways of writing could be considered variants. 

## How to use BCP-47 codes for your variant

BCP codes are a way of representing variation in languages and of being able to refer to specific variants, either written or spoken. The codes are important so that we have a way of distinguishing between different variants of the same language. A BCP code as used by Common Voice is made up of a maximum of four parts:

1. a language tag: This should be a two letter or three letter tag from ISO-639, for example ig for igbo or vot for Votic. These should be in lowercase.
2. an optional script tag: This should consist of four letters, be written in title case and chosen from ISO-15924. For example: Latn (Latin), Cyrl (Cyrillic), Deva (Devanagari), Beng (Bengali), Arab (Arabic).
3. an optional region tag: This should consist of two letters in capitals from XXX
4. an optional variant tag: These should be five to eight letters long, written in lowercase and are free to be made up by the community. For example: valencia (Catalan spoken in Valencia) or aranese and gascon for the Aranese and Gascon variants of Occitan respectively.

Some examples:

- es-MX: Spanish, as spoken in Mexico in Latin script. The script tag is left out as Spanish is only written in Latin script and no variants are specified.
- ca-valencia: The Valencian variant of Catalan. The script tag and country tag because Valencian is only written in Latin script in Spain.
- sr-Latn-ijekavsk: Serbian written in Latin script, spoken in Serbia and with the ijekavian variant (e.g. writing and pronouncing rijeka “river” instead of reka). This variant is spoken both in Serbia and Bosnia-Herzegovina but with few differences so the region tag is left out.
- rm-vallader: The Vallader variant of Romansch. Romansch is only spoken in Switzerland and only written in Latin script so the region and script codes are left out.
- pa-Guru: Punjabi written in Gurmukhi script. This variant is mostly used in India,  

In principle any redundant information should be left out, for example for English it is not necessary to add the Latn script tag, as English is only written in Latin script. For Valencian it is not necessary to add the ES region code as it is only spoken inside Spain. Note however that for some diaspora communities these may be relevant.

### List of useful resources

Wikipedia pages (in English):
- Language codes (ISO-639-3): https://en.wikipedia.org/wiki/ISO_639-3 
- Variant codes (BCP-47): https://en.wikipedia.org/wiki/IETF_language_tag
- Script codes (ISO-15924): https://en.wikipedia.org/wiki/ISO_15924
- Country and region codes (ISO 3166): https://en.wikipedia.org/wiki/ISO_3166-1

Other pages:
- Look up language codes: https://iso639-3.sil.org/code_tables/639/data/all
- BCP-47 specification details: https://tools.ietf.org/search/bcp47 

