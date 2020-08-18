# kanjobal-bilingual-corpus
Ugur Yavuz, August 2020

This is a Kanjobal-English bilingual corpus I compiled during my internship at the [Natural Language Group @ ISI](https://nlg.isi.edu/) under the supervision of Dr. Jonathan May.

## Structure
* `kjb-en` contains a Kanjobal (ISO: kjb) corpus of roughly 8310 sentences/Bible verses and ~11720 distinct tokens. It was compiled using the Kanjobal Bible available on [bible.is](https://live.bible.is/bible/KJBSBG/), and a Pedro Miguel Say's book [**Ikʹtiʹ yuu naj pel mekel ana**](https://www.worldcat.org/title/ikti-yuu-naj-pel-mekel-ana-cuentos-de-don-pedro-miguel-say-dibujos-de-virves-garcia-traduccion-y-redaccion-de-fernando-penalosa-et-al/oclc/28421867&referer=brief_results) which I have scanned using [Tesseract](https://tesseract-ocr.github.io/) and manually aligned by sentence/sentence-like fragments. 
* `knj-en` contains an Akateko (also known as Eastern Kanjobal, ISO: knj) corpus of roughly 30016 sentences/Bible verses and ~19790 distinct tokens. It was compiled using the Akateko Bible available on [bible.is](https://live.bible.is/bible/KNJAEM/).
* Each directory is divided into `corpus`, `documents`, and `metadata` subdirectories.
  * `corpus` contains plaintext versions of the corpus in each language under `plaintext`, and document, line number, and classification (genre) annotated .csv version of the corpus under `csv`.
  * `documents` contains the original documents.
  * `metadata` contains information about the translation pairings of documents in `pairs.csv`, and metadata information about each document in `documents.csv`.

## Notes
- On [bible.is](https://live.bible.is), there are numerous chapters of the Bible where verse numbers don't match between English and Kanjobal editions. In most cases, this is due to certain adjacent English verses being merged into a previous verse to form a single verse in Kanjobal. The alignment takes this into account.
