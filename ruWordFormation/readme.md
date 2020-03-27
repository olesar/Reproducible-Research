## Word Formation data for Russian

This is the core part of the data used in the annotation of the Rissian National Corpus. Here you can find two versions of the dataset, `morphodictKE1986.csv` and `morphodictKE1986.txt`.

* `morphodictKE1986.csv` is based on Kuznetsova & Efremova's comprehensive Dictionary of Russian morphemes (ca 52K words).
Example:
```
автобиографический;авто;корень;1;;A
автобиографический;био;корень;2;;A
автобиографический;граф;корень;3;;A
автобиографический;еск;суффикс;5;;A
автобиографический;ич;суффикс;4;;A
```
* Each row has a structure:
    + lemma; 
    + morph; 
    + label {корень - root; суффикс - root; префик - root; флексия - ending (optional)}; 
    + Nr. in the ordered list of morphemes of the lemma; 
    + a list of allomorphs, e.g. '2нос|наш|нес|нош';  
    + part of speech  
  
The word formation nest can be obtained using the list of allomorphs.   


* `morphodictKE1986.txt` is another version adopted for processing with Python by Maria Ignashina. 
Example: 
```
автобиографический,"['авто', 'био', 'граф', 'ич', 'еск', 'ий']","['авто', 'био', 'граф']",A,"[0, 4, 7, 11, 13, 16]","[[0, 3], [4, 6], [7, 10]]"
```
* Each row has a structure:
  * lemma  
  * a list of morphemes  
  * root (a list of roots)  
  * part of speech  
  * initial position of each morpheme (in characters)  
  * initial and final position of the root(s)  




### Publications

*  Grishina, Elena, Itkin, Ilya, Lyashevskaya, Olga, Tagabileva, Maria. O zadachax i metodax slovoobrazovatel'noj razmetki v korpuse tekstov. In: Poljarnyj Vestnik, Vol. 11, 2008. p. 38-46. 
[In Russian: Е. А. Гришина, И. Б. Иткин, О. Н. Ляшевская, М. Г. Тагабилева. О задачах и методах словообразовательной разметки в
корпусе текстов // Полярный вестник. 2009. Вып. 12. С. 5-25.]


### References

* A.I. Kuznetsova & T.F. Efremova, A Dictionary of Russian Morphemes, Moscow, 1986 [in Russian, Кузнецова, Ариадна Ивановна; Татьяна Фёдоровна Ефремова. Словарь морфем русского языка: около 52,000 слов. Москва: Русский язык, 1986.] [sample pages](KuznetsovaEfremova1986sample.pdf)
