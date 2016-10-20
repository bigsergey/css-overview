# An overview of CSS in 2016

## Introduction

W dziesiejszych czasach Frontend technologie rozwijają się bardzo szybko. Powstaję coraz więcej nowych podejść, metologii, bibliotek, framewroków itd. Wraz z javascriptem również się rozwija CSS. CSS pozwala na tworzenie pięknych stron. Pisanie styli w projektach zawsze było trudnym zadaniem. Niektóre cechy CSS robiące z niego potężne narzędzie w tym samym czasie powodują, że nasze style robią się legacy codem trudnym w utrzymaniu. W tym artykule postarałem się zebrać najbardziej znane narzędzia pozwalające na polepszenie pracy programista związanej z pisaniem styli.  

Narzędzia opisane w artykule są rozbitę na grupy, natomiast to tylko orientacyjny podział. Niektóre narzędzia ciężko jest wydzielić do jednej grupy. Z tym podziałem możecie się zgodzić lub nie, albo zaproponować własny (chętnie się dowiem wasze zdanie na ten temat). Głownym celem tego artykułu jest pomoc developerom zastanwiającym się z czego można skorzystać przy rozpocięciu pisania albo utrzymaniu styli w projekcie. 

## Preprocessors

Preprocessory CSS są jednym z najbardziej popularnych i wykorzystywanych narzędzi CSS. CSS preprocessor jest rozszerzeniem(extends) języka CSS, która dodaje wcześniej niedostępne możliwości w CSS, za pomocą nowych konstrukcji syntaktycznych. Preprocessory przekształcają kod napisany w składni preprocessora na poprawny CSS kod. Najbardziej znanymi preprocessorami są:

- [SASS](http://sass-lang.com/) - pojawił się w 2007 roku jako moduł do HAML i jest napisany w Ruby. Posiada dwie składni: Sass (Syntactically Awesome Style Sheets) i Scss (Sassy CSS).
- [LESS](http://lesscss.org/) - został utworzony przez [Alexisa Selliera](https://github.com/cloudhead) w 2009 roku i jest napisany w JavaScript (pierwotnie był napisany w Ruby).
- [Stylus](http://stylus-lang.com/) - najmłodszy z preprocessorów. Został zaimplementowany przez TJ Holowaychuka w 2010 roku. Jest napisany w Javascript. Obsługuje wiele różnych składni. 

W internicie można znaleźć dużo informacji na temat preprocessorów CSS. Głównie preprocessory mają następujące funkcje:

- Variables,
- Nesting,
- Mixins,
- Extends,
- Color operations,
- If/Else Statements,
- Loops, 
- Math,
- Imports.

Opis wyżej wymienionych funkcji i róznice w syntax dla preprocessorów SASS, LESS, Styles są bardzo dobrze opisane w artykule: [An Introduction to CSS Pre-Processors: SASS, LESS and Stylus](http://htmlmag.com/article/an-introduction-to-css-preprocessors-sass-less-stylus).



