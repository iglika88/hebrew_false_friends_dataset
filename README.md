# Hebrew False Friends Dataset

This dataset includes 50 homographs that exist in both Ancient (Biblical) and Modern Hebrew but have significantly different meanings. The dataset may be suitable for automatic model evaluation as well as academic/educational applications.

The pairs were derived through a crawl of Biblical and Modern Hebrew dictionaries and the calculation of cosine distance based on the words' English definitions as represented by two transformer models.

## Dictionary resources

Biblical Hebrew lexical data were extracted from:

- **Open Scriptures Hebrew Lexicon (Brown–Driver–Briggs Hebrew and English Lexicon)**  
  https://github.com/openscriptures/HebrewLexicon

Lemma forms were obtained from the accompanying **LexicalIndex.xml** index.

Modern Hebrew lexical items were obtained from:

- **Kaikki.org Hebrew dictionary dataset**  
  https://kaikki.org/dictionary/Hebrew/

Derived from Wiktionary using:

- **Wiktextract**  
  https://github.com/tatuylonen/wiktextract

## Semantic distance calculation

Cosine distance between dictionary definitions was calculated using two transformer models:

- **all-MiniLM-L6-v2** (English sentence transformer)  
  https://huggingface.co/sentence-transformers/all-MiniLM-L6-v2

- **distiluse-base-multilingual-cased-v2** (multilingual sentence transformer)  
  https://huggingface.co/sentence-transformers/distiluse-base-multilingual-cased-v2

## Files

- **false_friends_BH_vs_MH_final.xlsx**  
  Dataset in Excel format.

- **false_friends_BH_vs_MH_final.csv**  
  Dataset in CSV format.
