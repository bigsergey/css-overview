# An overview of CSS in 2016

## Introduction

W dziesiejszych czasach Frontend technologie rozwijają się bardzo szybko. Powstaję coraz więcej nowych podejść, metologii, bibliotek, framewroków itd. Wraz z javascriptem również się rozwija CSS. CSS pozwala na tworzenie pięknych stron. Pisanie styli w projektach zawsze było trudnym zadaniem. Niektóre cechy CSS robiące z niego potężne narzędzie w tym samym czasie powodują, że nasze style robią się legacy codem trudnym w utrzymaniu. W tym artykule postarałem się zebrać najbardziej znane narzędzia pozwalające na polepszenie pracy programista związanej z pisaniem styli.  

Narzędzia opisane w artykule są rozbitę na grupy, natomiast to tylko orientacyjny podział. Niektóre narzędzia ciężko jest wydzielić do jednej grupy. Z tym podziałem możecie się zgodzić lub nie, albo zaproponować własny (chętnie się dowiem wasze zdanie na ten temat). Głownym celem tego artykułu jest pomoc developerom zastanwiającym się z czego można skorzystać przy rozpocięciu pisania albo utrzymaniu styli w projekcie. 

## CSS Preprocessors

Preprocessory CSS są jednym z najbardziej popularnych i wykorzystywanych narzędzi CSS. CSS preprocessor jest rozszerzeniem(extends) języka CSS, która dodaje wcześniej niedostępne możliwości w CSS, za pomocą nowych konstrukcji syntaktycznych. Preprocessory przekształcają kod napisany w składni preprocessora na poprawny CSS kod. Najbardziej znanymi preprocessorami są:

- [SASS](http://sass-lang.com/) - pojawił się w 2007 roku jako moduł do HAML i jest napisany w Ruby. Posiada dwie składni: Sass (Syntactically Awesome Style Sheets) i Scss (Sassy CSS).
- [LESS](http://lesscss.org/) - został utworzony przez [Alexisa Selliera](https://github.com/cloudhead) w 2009 roku i jest napisany w JavaScript (pierwotnie był napisany w Ruby).
- [Stylus](http://stylus-lang.com/) - najmłodszy z preprocessorów. Został zaimplementowany przez [TJ Holowaychuka](https://github.com/tj) w 2010 roku. Jest napisany w Javascript. Obsługuje wiele różnych składni. 

W internicie można znaleźć dużo informacji na temat preprocessorów CSS. Głównie preprocessory mają następujący zestaw funkcji:

- Variables,
- Nesting,
- Mixins,
- Extends,
- Color operations,
- If/Else Statements,
- Loops, 
- Math,
- Imports.

Opis wyżej wymienionych funkcji i róznice w syntax dla preprocessorów SASS, LESS, Styles są bardzo dobrze opisane w artykule: [An Introduction to CSS Pre-Processors: SASS, LESS and Stylus](http://htmlmag.com/article/an-introduction-to-css-preprocessors-sass-less-stylus). Natomiast w tym artukule jak mówi nazwa są opisane 6 róznych preprocessorów CSS: [6 Current Options for CSS Preprocessors](https://www.sitepoint.com/6-current-options-css-preprocessors/).

## CSS Post(?)processors

Postprocesor CSS przymuje na wejście CSS, następnie przekształca go na różne sposoby i na wyjście podaje CSS. Przykłady postprocesorów:

- [CSSO](https://github.com/css/csso) - minifikacja CSS,
- [Pleeease.io](http://pleeease.io/) - aplikacja Node.js, która w prosty sposób przetwarza CSS.
- [CSSComb](http://csscomb.com/) - automatycznie zmienia formatowanie styli CSS i kolejność reguł w selectorach.
- [Rework](https://github.com/reworkcss/rework) - narzędzie pozwalające na manipulacje z CSS, udostępnia wygodny interfejs do stworzenia własnych pluginów przetwarzających CSS kod. Autorem jest TJ Holowaychuk (autor Stylus). Rework został zaprezentowany publicznie w 14 marca 2013 roku - [Modular CSS preprocessing with rework](http://tjholowaychuk.tumblr.com/post/44267035203/modular-css-preprocessing-with-rework).
- [PostCSS](http://postcss.org/) - narzędzie do transformacji(transforming) stylów za pomocą pluginów napisanych w Javascript. Autorem jest [Andrey Sitnik](https://github.com/ai). PostCSS jest oparty o idee Rework.

![Preprocessing and postprocessing in a toolchain](https://cdn-images-1.medium.com/max/1600/1*9WXGWDhXyzd5XGY1uz1nrg.jpeg "reprocessing and postprocessing in a toolchain")
**Rysunek 1.** *Preprocessing and postprocessing in a toolchain. Source: [Deconfusing Pre- and Post-processing](https://medium.com/@ddprrt/deconfusing-pre-and-post-processing-d68e3bd078a3#.l1kwsfwqv).*

A propo terminu 'postprocesor CSS' są różne opinie. Jedni uważają, że termin lepiej się nadaje do narzędzi, które działają w przeglądarce (np. [-prefix-free](http://leaverou.github.io/prefixfree/) lub client-side polyfills), drudzy mowią o postprocesorach jako o narzędziu, ktore pracuje bezpośrednio z css napisanym ręcznie lub wygenerowanym przez preprocesory (Rysunek 1). Na przykład zespół PostCSS zrezygnował z użycia terminu postprocessor i obecnie używają określenia processor CSS (oficjalny [tweet](https://twitter.com/PostCSS/status/626046993006239744) zepołu PostCSS). W tym artykule używamy określenia postprocessor.

Najbardziej znanym obecnie postprocesorem jest PostCSS. Posiada ponad 300 pluginów, jakość, popularność pluginow jest różna. Lista dostępnych pluginów można znaleźć na stronie [postcss.parts](http://postcss.parts/). Kilka przykładów:

- [Autoprefixer](https://github.com/postcss/autoprefixer) - najbardziej znany plugin PostCSS, który za pomocą wartości z serwisu [Can I Use](http://caniuse.com/) dodaje prefiksy do reguł CSS (add vendor prefixes to CSS rules).
- [cssnano](http://cssnano.co/) - plugin zajmujący się kompresją CSS kodu. 
- [Stylint](http://stylelint.io/) - analizuje kod CSS na obecność w nim błędów, a także trzymanie się przyjętego codestyle. 
- [RTLCSS]()
- [PreCSS]()
- [SugarSS]()
- [CSS Modules]()
- [postcss-cssnext]()
- [postcss-assests](), [postcss-inline-svg](), [postcss-sprites]().

Webpack używa PostCSS dla pracy z CSS.



