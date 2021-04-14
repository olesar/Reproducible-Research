## Universal Dependencies for pre-modern Russian: Morphology

We present the RNC Middle Russian, a historical corpus of the Russian National Corpus, annotated according to the Universal Dependencies (UD v.2) scheme (Zeman et al. 2019).

Firstly, we outline the UD tagset for parts of speech and morphological features and discuss key differences between the UD and RNC tagsets. As an illustration, we address several annotation templates such as named entities and periphrastic verb forms.

Secondly, for the corpus of ca. 10 million tokens, we propose a model for incremental semi-manual annotation. Starting from a small number of 'seed' texts annotated manually from scratch and the remaining part annotated automatically by a 'noisy'  model, we apply a correction strategy in order to:

(i) improve the quality of the training data up to the 'silver' level via correction templates;

(ii) improve the consistency of manual annotations;

(iii) improve the accuracy of the tagging model; and

(iv) increase the amount of 'gold' data. 

As a result, we gradually tip the balance between the poorly annotated training data and more and more reliably annotated test data  in favor of the latter. Moreover, as the behaviour of the accuracy metric clearly depends on the quality, amount, and representativeness of the test data with respect to the training set, our approach makes this metric more conservative yet more reliable in the task of tagging raw texts. 
