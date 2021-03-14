# Group Orange 🍊
Project Big-Scale Analytics - University of Lausanne


## Project Description 📝
This project aims at building a model for predicting the level of difficulty of a French text for native English speakers interested in learning French and wanting to improve their reading skills in French as a foreign language. The level of difficulty could then be used in a recommendation system, to recommend texts at the appropriate level for French learners. It has been shown that learners progress more easily if they read texts that are at the just right level of difficulty, rather than being presented with a text that has too many new words, or too little.

In this project we collected a set of labelled data for French learners, on which we will apply a natural language processing model to estimate the level of difficulty of unseen French sentences.

## Method 💡

## Data 📊
The dataset to train and test the model include labeled sentences in French. We collected a set of over 1000 annotated sentences, while keeping a balance in the difficulty levels from A1 to C2 (using as a reference the Common European Framework of Reference, CEFR). The sentences come from a rich mix of sources such as annotated exam preparation papers, corrected grammar exercises from text books, labelled newspapers and transcripts of radio interviews:
- http://www.delfdalf.fr/
- https://www.courrierinternational.com/
- https://savoirs.rfi.fr/en/recherche/rubrique/apprendre/thematique/culture-2717
- La Grammaire des Premiers Temps B1-B2, corrigés

We performed some preliminary cleaning of the data, removing incomplete sentences, correct spelling mistakes and removing copyright and other information included in the labelled French text, but that did not include actual French sentences.

## Related Work/ literature review 📚
Our review of the literature found that what makes a text more readable depends on the needs and characteristics of the target readers (Xia, Kochmar and Briscoe, 2016). Depending on the target audience, one might choose some readability criteria over others. The case of adult foreign language learners is different from say the case of adolescent native speakers. Xia and colleagues argue that this aspect needs to be taken into account account when collecting the labelled data for training the model. It is better if the collected texts and sentences correspond to text labelled for the purpose of teaching/learning French as a second language, which corresponds with our approach.

Still with the target audience in mind, we noted that Vlachos ad Lappas (2011) made reference to language cognates, meaning words that are similar in meaning and form between, in our case, French as the language to be learnt and English as the native language of the learner. 

A generic framework that asseses the level of difficulty of a foreign text can include several measures of readability and of familiarity (Vlachos and Lappas, 2011). Xia and colleagues provide a thorough overview of readability measures, such as: number of sentences per text, average and maximum number of words per sentence, average number of characters per word, average number of syllabels per word, which combined give the Flesch-Kincaid score and/ or the Coleman-Liau readability formula. To these traditional measure they add vocabulary knowledge and grammatical aspects. Vocabulary can be approximated with a corrected type-token ratio (TTR), which takes into account the number of unique words to the total number of words in a text, or by using part of speech (POS) and lexical variation or lexical density measures (such a the proportion of classes of lexical items - nouns, verbs, adjectives, adverbs, prepositions - in all words). The grammatical complexity of text can be measured by RAPS parser output, average number of noun, verb, adjective, adverb, perpositon clauses per sentence. Vlachos and Lapps (2011) define familiarity as a combination of popularity (words frequently used in a reference corpus of language) and cogantivity (words one can easily recognize as they are very similar in English and in French). Conceptual cognition difficulty can also affect the perceived difficulty of a text (whether the reader is familiar with the topic), as well as measures of text cohesion and coherence (Xia Kochmar and Briscoe, 2016). 

## Bibliography
François (2015). When readability meets computational linguistics: a new paradigm in readability, Rev. franç. de linguistique appliquée, 2015, XX-2 (79-97).

Vlachos and Lappas (2011). Ranking German Texts by Comprehensibility for Foreign Document Retrieval. SIGIR 2011 Workshop on Enriching Information Retrieval (ENIR 2011), July 28, 2011, Beijing, China.

Xia, Kochmar and Briscoe (2016). Text Readability Assessment for Second Language Learners. Proceedings of the 11th workshop on Innovative Use of NLP for Building Educational Applications, San Diego, California, June 16, 2016.
