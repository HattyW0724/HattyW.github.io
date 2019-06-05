# Research project(s) Qile contributed by using computational research approaches/data-driven skills

This page is to introduce the recent studies I contributed to by using server log analysis, web scraping, preliminary data analysis and visualization.

## 1. PPR Scheme: a exploratory media analysis - set The New York Times as example

###1.1. Background: 
  
  Today, global children and adolescents are growing up with the rapid change of digital age, and the need for digital literacy is increasingly shaping young people’s life and learning (Linebarger & Piotrowski, 2009; Flewitt, 2011; Alper, n.d.). “For better and for worse, digital technology is now an irreversible fact of our lives,” quoted Anthony Lake, Executive Director of the United Nations International Children’s Emergency Fund (UNICEF, 2017, p.v), and with a kaleidoscope of functions, mobile phone, especially smartphone, has become an integral part of social and daily life for children and adolescents in the digital age. Like other digital devices, smartphones are becoming “the tools for communication, collaboration, social networking, and user-generated content” (NAEYC & Fred Rogers Center, 2012) for young. However, according to “¬¬”, which is one of UNICEF’s annual publication uncovering the role of digital technology in helping and hindering global children’s learning and well-being, young people have relied excessively on smartphones to go online, in comparison with other digital devices such as desktops, laptops, tablets and games consoles.  In addition, “the Global Kids Online Research Synthesis 2015-2016”, published by UNICEF Office of Research – Innocenti, also found that “children predominantly and mostly access the internet at home through smartphones” (UNICEF & Byrne et al., 2016, p.8).  
 
 ![Alt text](https://github.com/HattyW0724/HattyW.github.io/blob/master/%5Bgap%5D%20Systematic%20reviews%20about%20adolescents'%20phone%20use%20.png "Literature review about the academic's concerns")

  
  As the essential role speaking out the voice of digital use's importance, how professional media insights about the issue can reflect vividly about society's concern and the stockholders attitudes who are from diverse corners in society.
  For a better understanding about the society's careness about digital youth's digital or social media use, and make a pre-test for further study on the correlation between media's broadcast and views from parents,educators as well as academys, as the research assistant in the Department of Education Studies, HKBU, I made a preliminary and exploratory analysis, setting The New York Times as example.
  
###1.2. Approaches:

> 1.   **Python** with modules to do web scraping, preliminary content analysis (word frequency AND part of speach labels) and data visualization
> 2.   **Tableau**
> 3.   **Nvivo** to do qualitative sentimental analysis


**Information Collection: Web scraping from the New York Times**

Data source: NYT's official <a href="https://developer.nytimes.com/">API</a> AND the module requests()

******Data Collection******
> 1.  keyword: "social+media"
> 2.  Time span: Default
> 3.  Sample capacity: 150 items

<pre><code>
====================
&gt; api_url = 'https://api.nytimes.com/svc/search/v2/articlesearch.json?q=social+media&page=3&api-key=2J6odNdJ0Ui0WUzOamvvk4NmCtbG1W50'
&gt; response = requests.get(api_url)
&gt; data_# = response.json() # 10 items per page, 1 page per time.
</code></pre>


### 1.2. Premilinary analysis

(omit)

**Top 30 frequenciest word in the data**
 keywords  frequency
> 0.        media         65
> 1.       social         63
> 2.     facebook         27
> 3.       people         18
> 4.         week         13
> 5.      twitter         13
> 6.         news         11
> 7.         tech         11
> 8.        times         11
> 9.      company         11
> 10.   instagram         10
> 11.       video         10
> 12.    internet         10
> 13.   president          9
> 14.       trump          9
> 15.        york          9
> 16.       women          9
> 17.   platforms          8
> 18.       month          8
> 19.      health          7
> 20.    industry          7
> 21.     tuesday          7
> 22.      online          7
> 23.         ago          7
> 24.   political          7
> 25.     readers          7
> 26.     million          7
> 27.        past          6
28       world          6
29    accounts          6

![Alt text](NYT_wordcloud.png “<p>wordcloud.WordCloud()</p> to show the word frequency")


### 1.3. Advanced analysis

Via Nvivo, I did sentimental analysis (negative/positive) about the content 

![Alt text](https://github.com/HattyW0724/HattyW.github.io/blob/master/Matrix%20Coding%20Query%20-%20Results%20Preview%20.jpg "Sentimental analysis via Nvivo")
  

## 2. Other studies I have contributed

![Alt text]（Image from WangQile_Citizen Journalism and Professional Journalism (1) copy, page 15.png "**Map** Professional Journalism vs Citizen Journalism on Twittersphere - #breakingnews")

> 1.  Wang, Q., Zhang, X., & Man, Z. (2018). Survey of content production in Hong Kong Media.
In Li, R. & Huang, Y. (eds), Hong Kong digital media development report 2018 (pp. 224–247). Hong Kong: Chung Hwa Press.
> 2.   <a href="https://github.com/HattyW0724/HattyW.github.io/blob/master/WANG%20Qile%20_PJ%26CJ.pdf">API</a> （Individual course project)
> 3.  
