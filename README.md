# Key-Phrase-Extraction-and-ranking-tweets
Pulling tweets via API, KPE using directed graphs, and ranking using twitter metrics
Firstly tweets were pulled using the twitter API; tweepy was used to streamline this process. Public metrics were also pulled through API including likes, retweets, and views. Then tweets are preprocessed and NetworkX is used to build a directed network representation, and inbetweeness was used as the centralitly measure to rank words/nodes in graph. Key words were defined as top 100 words by centrality measure. Key phrases were pulled from the processed tweets, KP being defined as sequence of key words with a length >= 2. Then keyphrases were ranked intially by sum of likes by tweet containing KP. Intial experimenting with this process using "ukraine" as API query resulted in the following graph. (Due to size restraints only a subset of graph is available)
![my_graph](https://user-images.githubusercontent.com/106636917/213756254-82844b98-52ac-409e-8bda-b2b948691692.png)

After KPE and ranking the resulting ranked phrases (by likes) showed the top 3 all pertain to Denmarks dontation of tanks to the war efforts. This anlaysis was only done using a very small sample of tweets; roughly 100. 
The jupyter notebook in this repository has all necessary cells to replicate the process. 
