# Assignment_2_Analogies
According to the parallelogram model, two pairs of words (A: B and C: D) are relationally similar to the extent that their difference vectors (vB − vA and vD − vC) are similar. [3]

There are some caveats. For example, the closest value returned by the parallelogram algorithm in word2vec or GloVe embedding spaces is usually not in fact b* but one of the 3 input words or their morphological variants (i.e., cherry:red :: potato:x returns potato or potatoes instead of brown), so these must be explicitly excluded. [1]

Furthermore while embedding spaces perform well if the task involves frequent words, small distances, and certain relations (like relating countries with their capitals or verbs/nouns with their inflected forms), the parallelogram method with embeddings doesn’t work as well for other relations (Linzen 2016, Gladkova et al. 2016, Schluter 2018, Ethayarajh et al. 2019a), and indeed Peterson et al. (2020) argue that the parallelogram method is in general too simple to model the human cognitive process of forming analogies of this kind. [1]

the analogy dataset proposed by Mikolov et al. (2013a). This dataset, which has become a standard VSM evaluation set (Baroni et al., 2014; Faruqui et al., 2015; Schn- abel et al., 2015; Zhai et al., 2016), contains 14 categories; see Table 1 for a full list. A number of these categories, sometimes referred to as “syntactic”, test whether the structure of the space captures simple morphological relations, such as the relation between the base and gerund form of a verb (scream : screaming). Others evaluate the knowledge that the space encodes about the world, e.g., the relation between a country and its cur- rency (latvia : lats). A final category that doesn’t fit neatly into either of those groups is the relation between masculine and feminine versions of the same concept (groom : bride). [2]

Based on [4]: 
a)  inflectional morphology is overall easier than semantics
b) surprising that derivational morphology is significantly more difficult to detect than inflectional 
c) lexicographic relations are very difficult to detect with the vector offset method d) the easiest category is binary antonyms of the up:down kind - the category for which the choice should be the most obvious in the semantic space. -> derivational and lexicographic relations remain a major challenge.

References

[1] Jurafsky, D. and Martin, J.H. (2008) Speech and Language Processing: An Introduction to Speech Recognition, Computational Linguistics and Natural Language Processing. Prentice Hall, Upper Saddle River, NJ.

[2] Linzen, T. (2016). Issues in evaluating semantic spaces us- ing word analogies. 1st Workshop on Evaluating Vector- Space Representations for NLP.
https://aclanthology.org/W16-2503/


[3] Peterson, J. C., Chen, D., & Griffiths, T. L. (2020). Parallelograms revisited: Exploring the limitations of vector space models for simple analogies. Cognition, 205, Article 104440. https://doi.org/10.1016/j.cognition.2020.104440
https://cocosci.princeton.edu/papers/peterson_parallelograms.pdf

[4] Rogers, Anna & Drozd, Aleksandr & Matsuoka, Satoshi. (2016). Analogy-based detection of morphological and semantic relations with word embeddings: what works and what doesn't.. 8-15. 10.18653/v1/N16-2002. 
https://www.researchgate.net/publication/305334369_Analogy-based_detection_of_morphological_and_semantic_relations_with_word_embeddings_what_works_and_what_doesn%27t
