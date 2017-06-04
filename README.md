# indeed_tweets
Data Pipeline to output a visualization of the worldwide tweets from Indeed.com.
The final HTML can be viewed <a href='http:\\www.andresmack.com/indeed_tweets_visual.html'>here</a>
<ul>
<li><b><i>indeed_worlwide_tweets_getter</b></i> calls the Twitter API client (not uploaded here) to gather all the tweets from the different Indeed users around the world. Outputs .jsonl files.</li>
<li><b><i>tweet_consolidator</b></i> reads the jsonl files and consolidates the desired fields. Outputs a .txt file delimited by "|".</li>
<li><b><i>tweet_visualizer</b></i> finally grabs the .txt, converts into a pandas dataframe, and using bokeh + html, css, js, we get the final <a href='http:\\www.andresmack.com/indeed_tweets_visual.html'>visualization</a>.
<li>Pipeline was managed using luigi (not uploaded here)</li>
</ul>
