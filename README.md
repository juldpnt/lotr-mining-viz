# lotr-mining-viz

As a big fan of Tolkien's works I decided to highlight the links between the characters using statistical and computer tools.

### Data-mining

First of all, I needed data. I decided to learn data mining in order to obtain complete and quality databases. After testing a few sites, Tolkien Gateway was the most appropriate (complete data, characters well separated from each other on each page...)
This can be found in the data_scrapping file
<img src="https://github.com/juldpnt/lotr-mining-viz/blob/main/img/tolkien_gateway_home_page.png?raw=true" width ="25%" align="center">

### Data engineering, natural language processing

Then, we had to analyze the relationships. I was inspired by the work of Vincent Labatut and Xavier Bost (2019. Extraction and Analysis of Fictional Character Networks: A Survey . ACM Computing Surveys 52(5):89. https://doi.org/10.1145/3344548) and Thu Hien Vu sur YouTube.
The method of detecting interactions is that of Co-occurrences, on intervals decided according to the works (see the code) because all do not have the same scene unit (e.g. the hobbit is much shorter than the lord of the rings and denser for some co-occurrences).

### Network made with data 

This allowed us to create a network graph representing the co-occurrences of the different characters.
See below a graph made for the hobbit.
<div align="center">
<img src="https://github.com/juldpnt/lotr-mining-viz/blob/main/img/network.png?raw=true" width="50%">
<img src="https://github.com/juldpnt/lotr-mining-viz/blob/main/img/network%20-%20Copie.png?raw=true" width="50%">
</div>

### TODO: 

1) Refactor the code.
2) Make a separate file for data mining AND for data analysis.
3) Make the functions usable for all files respecting the nomenclature of the text files (typically, not having to make tweaks if you want to study the hobbit or lotr 1 file)
4) Provide a sample file for the usable books and remove the current files (for legal reasons)
