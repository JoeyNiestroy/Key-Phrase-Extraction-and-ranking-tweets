# Key-Phrase-Extraction-and-ranking-tweets
Pulling tweets via API, KPE using directed graphs, and ranking using twitter metrics
Firstly tweets were pulled using the twitter API; tweepy was used to streamline this process. Public metrics were also pulled through API including likes, retweets, and views. Then tweets are preprocessed and NetworkX is used to build a directed network representation, and inbetweeness was used as the centralitly measure to rank words/nodes in graph. Key words were defined as top 100 words by centrality measure. Key phrases were pulled from the processed tweets, KP being defined as sequence of key words with a length >= 2. Then keyphrases were ranked intially by sum of likes by tweet containing KP. Intial experimenting with this process using "ukraine" as API query resulted in the following grpah. (Due to size restraints only a subset of graph is available)[my_graph.pdf](https://github.com/JoeyNiestroy/Key-Phrase-Extraction-and-ranking-tweets/files/10468195/my_graph.pdf)
