# An exploratory media analysis - set The New York Times as example


## Background: 


![Alt text](https://github.com/HattyW0724/HattyW.github.io/blob/master/Alexa.png "Top 10 Most popular digital media platforms initiated by newspaper ")

Source: Alexa

### Why set New York Times as example:

"The New York Times began publishing daily on the World Wide Web on January 22, 1996, "offering readers around the world immediate access to most of the daily newspaper's contents." The website had 555 million pageviews in March 2005. The domain nytimes.com attracted at least 146 million visitors annually by 2008 according to a Compete.com study. In March 2009, The New York Times Web site ranked 59th by number of unique visitors, with over 20 million unique visitors, making it the most visited newspaper site with more than twice the number of unique visitors as the next most popular site. as of May 2009, nytimes.com produced 22 of the 50 most popular newspaper blogs. NYTimes.com was ranked 118 in the world, and 32 in the U.S. by Alexa on June 4, 2017." 

(Wikipedia: New York Times Website)

### Approaches:

> 1.   **Python** with modules to do web scraping, preliminary content analysis (word frequency AND part of speach labels) and data visualization
> 2.   **Tableau**
> 3.   **Nvivo** to do qualitative sentimental analysis


**Information Collection: Web scraping from the New York Times**

Data source: NYT's official <a href="https://developer.nytimes.com/">API</a> AND the module requests()

Data Collection

> 1.  keyword: "social+media"
> 2.  Time span: Default
> 3.  Sample capacity: 150 items

<pre><code>
&gt; api_url = 'https://api.nytimes.com/svc/search/v2/articlesearch.json?q=social+media&page=3&api-key=2J6odNdJ0Ui0WUzOamvvk4NmCtbG1W50'
&gt; response = requests.get(api_url)
&gt; data_# = response.json() # 10 items per page, 1 page per time.
</code></pre>


<a href="https://github.com/HattyW0724/HattyW.github.io/blob/master/adolescents'%20social%20media%20use_TheNewYorkTimes.ipynb">Json script translation</a>


### 1.2. Premilinary analysis


<div class='tableauPlaceholder' id='viz1559797357968' style='position: relative'><noscript><a href='#'><img alt=' ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Bo&#47;Book1_15597970487290&#47;Sheet1&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='Book1_15597970487290&#47;Sheet1' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Bo&#47;Book1_15597970487290&#47;Sheet1&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /></object></div>                <script type='text/javascript'>                    var divElement = document.getElementById('viz1559797357968');                    var vizElement = divElement.getElementsByTagName('object')[0];                    vizElement.style.width='100%';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';                    var scriptElement = document.createElement('script');                    scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';                    vizElement.parentNode.insertBefore(scriptElement, vizElement);                </script>


**Top 10 frequenciest word in the data (partially)**
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


note: by using NLTK package to analyze wordfrequency. <a href="https://github.com/HattyW0724/HattyW.github.io/blob/master/NYT_social_media_FreqDist%20(NLTK).ipynb">Code</a>



Development: using TF-IDF module to do advanced word frequency analysis.


![Alt text](https://github.com/HattyW0724/HattyW.github.io/blob/master/NYT_wordcloud.png “wordcloud.WordCloud to show the word frequency")


### 1.3. Advanced analysis

Via Nvivo, I did sentimental analysis (negative/positive) about the content :

![Alt text](https://github.com/HattyW0724/HattyW.github.io/blob/master/Matrix%20Coding%20Query%20-%20Results%20Preview%20.jpg "Sentimental analysis via Nvivo")
 
 
 Development: using 
 
 

### 1.4. Insights


