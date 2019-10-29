# L8_thesis_sample

My Master’s thesis involves a classification task in Python and Jupyter notebooks to perform a quantitative error analysis of language learner's production in English. The study involves observations of Spanish-speaking language learner errors from teachers in the classroom setting, proposed popular error types produced by Spanish-speaking English Language Learners in literature, and a classification task of error reporting through parallel distance edits using ERRANT (ERRor ANnotation Toolkit) using data from the Lang-8 corpus, a language exchange website. Additionally, I use Jupyter notebooks for data pre-processing and cleaning. It is anticipated that the resulting statistical analysis would benefit NLP (Natural Language Processing), CALL (Computer Assisted Language Learning), and Education communities.


# == Initial approach ==

- Created function "l8_en_sp_dataclean" that segements the data from the lang-8 corpus only from users who's home language was Spanish, and Target(learning) language is English.

- Created function l8_en_spanish_aligner to get an idea of which corrections aligned with which learner input, blank lists '[]' indicate no corrections were made.

- Made two separate lists: One for learner sentences, another for corrections

- Zipped lists together into a dictionary (l_c_dict), if there was an empty correction, learner input was duplicated into value of dictionary.

- Used a regex expression to Capture text within brackets([])

- Checked for number of Corrections vs. Non-Corrections

- Represented "l_c_dict" in pandas

# == Current Approach, Beginning from the 10th cell ==

- Read in cleaned learner and corrector sentences as distinct files (file_1 and file_2).
- Read in the error report generated by ERRANT (ERRor ANnotation Toolkit), stored as a list of lists.
- Generated dependencies for both learner and corrector sentences via SpaCy, stored as separate lists.
- Created a master that contains the following: 
[
[learner_sentence,
[learner sentence dependencies], 
corrector sentence,
[corrector_sentence_dependencies], 
[Error report for the given sentence generated by ERRANT] 
]

- The immediate next step is to use the depencies generated between learner / corrector sentence pairs to inform an analysis of instances of Pronoun dropping. The hypothesis being that transfer errors may influence instances of Pro-dropping to a degree. Other error type analysis to follow are: Word Order, Subject-verb agreement, and Tense.

# Entrainment of internet slang terms via Tweets for a Corpus Analysis course

This project dealt with the hypothesis that Twitter users entrain on one another through popular internet slang terms. Using Twitter API and a scraper, Original tweets using slang terms are compared to reply tweets to see how frequent is the case of entrainment.
