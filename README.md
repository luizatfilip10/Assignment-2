# Documentation
## Corpus description
This corpus consists of lyrics from six Sleep Token songs. The first three songs, Blood Sports, Dangerous, and Dark Signs, come from the band’s debut-era releases in 2019, while the latter three, Ghestomane, Look at Windward, and Sugar, are drawn from their most recent album released in 2025. All lyrics are in English and the goal of this dataset is to explore how Sleep Token’s lyrical style may have shifted over time, as well as to identify distinctive linguistic patterns across songs. The corpus of lyrics was taken from the website Genius.com
## Target audience
The target audience for this corpus includes students in linguistics or digital humanities who are learning to build small corpora and practice POS-based annotation using tools like spaCy. It is also relevant for researchers interested in the linguistic features of song lyrics, particularly those examining stylistic or thematic patterns across different creative periods. Lastly, fans or analysts of Sleep Token with an interest in lyric interpretation.
## Text selection
Six songs were selected for this analysis. Three from their first album (2019) and three from their latest album (2025). The choice of songs was based on its length, so the ones with the most text were chosen. 
## Data collection
Lyrics were collected from the website Genius.com and each song's lyrics were copy/pasted into plain .txt files into the data folder.
Metadata (title, album, artist and year) was compiled in a CSV file. 
## Cleaning and preprocessing 
No cleaning or preprocessing was done to the dataset
## Annotations
Using spaCy (en_core_web_sm), the following annotations were added:
1. Tokens
2. Lemmas
3. Parts-of-Speech (POS)
4. Proper nouns
5. Named entities
6. NE words
## Corpus format 
1. The raw .txt files of each song
2. The metadata.csv file: 

| Column Name  | Description | Data Type |
| ------------- | ------------- | ------------- |
| FILENAME  | name of the .txt file | text |
| TITLE  | title of the song  | text |
| ALBUM | the album each song belongs to  | text |
| ARTIST  | name of the band (Sleep Token) | text |
| YEAR  | year of release  | number |

3. The annotated_dataset.csv file contains:
   - Filename &rarr; name of the .txt file
   - Title &rarr;  title of the son
   - Album &rarr; the album each song belongs to
   - Artist &rarr; name of the band (Sleep Token)
   - Year &rarr; year of release
   - Text &rarr; the original text
   - Document &rarr; the preprocessed text for analysis
   - Tokens &rarr; the segmentated strings into individual words and punctuation markers
   - Lemmas &rarr; the retreived dictionary root word of each word
   - POS &rarr; includes the part-of-speech tag for each token (e.g., noun, verb, adjective, adverb)
   - Proper_Nouns &rarr; list of all tokens in each song that were tagged with the PROPN part-of-speech tag
   - Named_Entities &rarr; the entities identified by spaCy’s NER
   - NE_Words &rarr; the actual text strings of the named entities detected by spaCy
## Quality checks 
No quality check has been done for the corpus, the lyrics were copied and pasted as they were found from the website. 
