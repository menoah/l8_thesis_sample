# l8_thesis_sample

My Master’s thesis involves a classification task in Python and Jupyter notebooks to perform a quantitative error analysis of language learner's production in English. The study involves observations of Spanish-speaking language learner errors from teachers in the classroom setting, proposed popular error types produced by Spanish-speaking English Language Learners in literature, and a classification task of error reporting through parallel distance edits using ERRANT (ERRor ANnotation Toolkit) using data from the Lang-8 corpus, a language exchange website. Additionally, I use Jupyter notebooks for data pre-processing and cleaning. It is anticipated that the resulting statistical analysis would benefit NLP (Natural Language Processing), CALL (Computer Assisted Language Learning), and Education communities.

Sample code from my thesis project

- Created function "l8_en_sp_dataclean" that segements the data from the lang-8 corpus only from users who's home language was Spanish, and Target(learning) language is English.

- Created function l8_en_spanish_aligner to get an idea of which corrections aligned with which learner input, blank lists '[]' indicate no corrections were made.

- Made two separate lists: One for learner sentences, another for corrections

- Zipped lists together into a dictionary (l_c_dict), if there was an empty correction, learner input was duplicated into value of dictionary.

- Used a regex expression to Capture text within brackets([])

- Checked for number of Corrections vs. Non-Corrections

- Represented "l_c_dict" in pandas

- A few regex expressions for the cleaning of the meta-data present in the corpus

# Entrainment of internet slang terms via Tweets for a Corpus Analysis course

This project dealt with the hypothesis that Twitter users entrain on one another through popular internet slang terms. Using Twitter API and a scraper, Original tweets using slang terms are compared to reply tweets to see how frequent is the case of entrainment.
