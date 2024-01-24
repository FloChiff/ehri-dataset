<img src="https://www.memorialdelashoah.org/wp-content/uploads/2016/07/ehri-300x300.jpg" width="100" align=right>

EHRI Dataset
=====================

## License

CC-BY 4.0

## Description

This dataset is a mix of several corpus created as part of the EHRI project. It contains documents in various languages (english, german, polish, hungarian, slovak, danish and czech). There are four types of documents distributed among the different languages: early Holocaust testimonies, diplomatic reports on the persecution and murder of European Jews during World War II, documents about the deportation to Nisko and documents about the Austrian refugees on the border with Czechoslovakia in the crisis year of 1938.

## Extent

**ALTO XML files from various corpus, divided into 7 sub-corpus**

| # | name | nb of images | GT for segmenter? | GT for recognizer? | description |
| --- | :---- | :---: | :---: | :---: | :---: |
| 1 | czech | (46) | y | y | Typewritten documents in Czech, mostly with many tight lines |
| 2 | danish | (36) | y | y | Typewritten documents in Danish, standard layout |
| 3 | english | (54) | y | y | Typewritten documents in English, standard layout |
| 4 | german | (56) | y | y | Typewritten documents in German, mostly with many tight lines |
| 5 | hungarian | (30) | y | y | Typewritten documents in Hungarian, standard layout |
| 6 | polish | (15) | y | y | Typewritten documents in Polish, few with many tight lines and many with fading writing |
| 7 | slovak | (15) | y | y | Typewritten documents in Slovak, standard layout |

*The ground truth can be used for both segmenter and recognizer training, but the segmentation does not contain any regions, so the segmenter will only learn to create lines.*

## Transcription guidelines

This dataset contains text written with a typewriter, but there are also some handwritten additions in the margin at times. The choice was made to not take them into account, therefore they were not segmented. Furthermore, some lines contains strikethrough content at their beginning or end: likewise, the choice was to not fully segmented the line and stop after/before the crossing.

## Sources

The original documents are held at various places and countries:
- Archives of the Jewish Community (IKG) Vienna (Austria)
- Austrian State Archives (Austria)
- Danish National Archives (Denmark)
- Hungarian Jewish Archives (Hungary)
- Jewish Historical Institute in Warsaw (Poland)
- Jewish Museum in Prague (Czech Republic)
- Moravian State Archives (Czech Republic)
- National Archives and Records Administration II (United States of America)
- National Archives Prague (Czech Republic)
- The Vienna Library for the Study of the Holocaust and Genocide (Austria)
- Yad Vashem Archives (Israel)

## Models

This dataset was made to create a multilingual model, but single-language models were also created in parallel. They are available in the folder *models* with a [readme](https://github.com/FloChiff/ehri-dataset/models/README.me) detailing the number of documents/lines for each language, the source of the documents, and the model name and its accuracy.
