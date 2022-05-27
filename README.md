# kpop-korean-russian-corpus
Hi! This repository contains codes and files related to my course paper dedicated to creating a korean-russian corpus of k-pop texts.

Due to technical issues I had to host one half of the analysis in my Jupyter Notebook (the 1st part) and another part in Google Colab (the 2d part).  
Also I restructured meta information partially automatically and partially manually, so the resulting meta information in the processed files is somewhat different from the one I recieve when analyzing the web page.

## Description of contents
**K-pop songs analizer part 1.ipynb** downloads lyrics, translation and meta data from https://lyricstranslate.com/ru.  
For it to work one has to specify only the link of the page they want to download.  
The result will be a json file with a list, where the first element is a dictionary with meta data and the second element is a dictionary with lyrics and translation.

**K_pop_songs_analizer_part_2.ipynb** analyzes texts and structures them so that they fit the Tsakorpus format. 
For it to work make sure you have in your current directory:
- kor_rus_dict_heavy.json and kor_rus_dict_light.json, they contain dictionaries for translation
- hangul without readings.txt, it contains hangul symbols, which are used for identifying the language
*compelling a dictionary.ipynb* is the code I used to make up the two dictionaries from the two corresponding .pdf versions (not mine*).
In code itself you should only specify the name of the text file you're working with.

In **processed texts** you can see the result of the analysis. There are 84 texts now, but of course I plan to process more. 

## P.S.
Некоторые файлы были обновлены / загружены 27.05.22. Это было согласовано с научным руководителем.

I also have already made a version of K_pop_songs_analizer_part_2.ipynb which deals with many texts at once, so the code will be updated soon.

The folder *old* contains files I uploaded earlier and after I have my grade for the 2d year course paper, I will delete it.

\* One of the dictionaries was found on the Internet without any metadata. Another one is the following: 한러사전 / 발행인: 이상수, 한국러시아어문학회, 서울, 2002
