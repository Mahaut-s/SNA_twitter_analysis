# Twitter Analysis
INTRODUCTION
Mass shootings are a serious and ongoing issue in many countries, and they often lead to heated debates and discussions around gun control measures. That's why we decided to analyse one specific shooting, the one that unfortunately happened in Nashville, Tennessee on the last 27th of March of the current year 2023; specifically in the Covenant school.

This event went viral on social media platforms, like Twitter, which actually offers an opportunity to examine these discussions and to gain insight into public opinion on the matter. In this project we conducted an analysis on Twitter using hashtags to identify how people were talking about the Covenant school shooting. 

We also applied the Louvain Method, which is a community detection algorithm that uses modularity optimization to identify clusters or communities in networks.Thus, we used it in order to identify clusters of tweets that are predominantly Pro or Anti-gun control with the goal of seeing if there is any polarization in public opinion

METHOD ＆ PROCESS
There are two key points about the clustering method: first, how the clusters are defined, and second, how they are calculated.

First, clusters are defined using Modularity, an index of cluster quality calculated from the formula like this, as we learned from Newman and Girvan's paper in class. In this formula, the red part is the actual percentage of edges in a given cluster, and the green part is the percentage of edges in a random graph.

画像

So, what is the best way to actually detect communities using Modularity?　There are several methods for community detection: the Girvan-Newman method, which removes edges that are likely to be present in a cluster in a top-down fashion; the Newman method, which improves modularity from the bottom-up; the CNM method, which speeds up the Newman method by introducing heaps and using heuristics; and the Louvain method, which computes only between close nodes. Here, we decided to use the Louvain method, which is the least computationally intensive, fastest, and most accurate.

Based on these premises, here is the actual process.
Step 1, Scraping tweets
Here, we scraped 5000 tweets by referencing 30,000 tweets under certain conditions using the neutral and frequently used tag #NashvilleCovenantSchool.

Step 2, Building reply network
After that, we built a reply network and were able to visualize it based on the following four indicators.

And finally, Step 3, Building semantic network
In this step, we built a network in which we could see the relationship between hashtags. Using the Louvain method described earlier, we were able to detect several communities and analyze each of them.


ANALYSIS 

The results of the Louvain method does not show a direct polarization of opinions but rather a collection of different clusters. Some of these clusters lean towards a pro or anti gun stance while others clusters have no poitical opinions yet other themes can still be identified within them. 

Notably, even the political clusters are not entierley unanimous in their leaning and have hashtags within them that seem misplaced in relation to the general sentiments of the hashtags in that cluster. This may however be due to tweets which support one opinion but point to the hypocrisy of other opinions or use the hashtags of these other opinions ironically.

![SNA Final group project-1](https://user-images.githubusercontent.com/130977434/235372823-53755950-5a2b-4ec5-bd60-80c3f4cb8df5.png)


RED: One of the more prominent hashtags: 
#guncontrol, #guncontrolnow, #enoughisenough, #stopmassshooting, #assultweaponban, #secureourschools, #gundlawssavelives

#goplovesgunsmorethanourkids, #gopdoesnotcareifkidsdie, #gopisnottheprolifepartytheyareprodgundeath these all refer to the grand old part, synonymous with the republican party. As this cluster also has hashtags which encourage gun control and ban of weapons, one can assume that those who tend to be critical of the republican party will also be for gun laws. This will often be those who vote democrat due to americas two party system.

#prolife seems odd in the context but may be calling out hypocrisies of republicans who will often make prolife arguments in relation to abortion but not in relation to guncontrol. 

![SNA Final group project (1)-1](https://user-images.githubusercontent.com/130977434/235373450-4628c2f3-3aeb-4c1f-8fd1-06f21977d9ab.png)

BLUE: is also a more political cluster with different views to the red one. 
#tstandsforterrorist, #genderdysphoriaisanillness, #redflagtrans, #2ashallnotbeinfinged, #timburchette, #backtheblue, #transgenderproblems, #notthegunsfault
#liberalsmustgo, #liberalhypocrisy,#liberalismisacult, #liberalismisamentaldisorder, #democratsaredestroyingamerica This cluster is typically pro gun and anti liberal which opposes the red cluster. 
 #genderaffrimingcare and #mentalhealthawareness again seem out of place in the context of the other blue tweets but we cannot tell the context of these tweets and thereby cannot be sure if they align with the opinions of the cluster or not. 

![SNA Final group project (2)-1](https://user-images.githubusercontent.com/130977434/235373770-0b785e81-c0ef-4a5e-9615-458cd01df7df.png)

GREEN: is also political and typically pro gun control and critiques of the republican party. 
#anothershooting, #itsthegunsandtherepublicans, #banar15s, #stop, #gopdomesticterrorists, #saveourchildren, #gunsafteynow, #yourchildcouldbenext
#itsthegunsstupid which seems to be a direct response to the hashtag from thew blue cluster #notthegunsfault

![SNA Final group project (3)-1](https://user-images.githubusercontent.com/130977434/235373968-ce0486b5-599e-478d-8df7-51d6b9764296.png)

TURQUOISE: does not seem to have a political leaning or stance on gun voilence but is more about themes of religion and charity. Notably, not just christianity is mentioned. 
#bible, #pray, #christian, #jesusislord, #ramadan, #jesus, #christianity, #givingtuesday

![SNA Final group project (4)-1](https://user-images.githubusercontent.com/130977434/235374134-729becbc-ab8e-461d-987b-5aa21fe4ccca.png)


PURPLE: contains a range of hastags but many of them are references to other shootings that have occurred.
#buffalomassacre, #parklandmassacre, #virginashooting, #columbine, #elpasoshooting, #dadeville, #sandyhook

![SNA Final group project (5)-1](https://user-images.githubusercontent.com/130977434/235374352-cd833826-b189-4654-ba65-fefdc0dffdb6.png)


Some clusters have seeminly nothing to do with the theme of gunvoilence but concern other relevant topics such as #nft or #ukraine. This may be linked to social media culture and an attempt to gain exposure through trending hashtags despite their relevance to the topic of the tweet. 







CONCLUSION


In conclusion, this analysis can’t show polarization but helps us to identify how people are talking about a recent mass shooting. To do so, we use the Louvain community iGraph algorithm that allows us to identify clusters with mostly pro-gun control tweets and to some extent anti-gun control tweets.

To further analyze our results, we compare them to existing surveys which were made by experts using machine learning to analyze reactions on Twitter about the Sandy Hook Elementary school shooting (Wang, N., Varghese, B., & Donnelly, P. (2017). A Machine Learning Analysis of Twitter Sentiment to the Sandy Hook Shootings. ) We can notice the recurrences of some hashtags on Twitter after a mass shooting like #PrayFor  or #guncontrol  that builds a social media culture that automatically give people some conventions while expressing their emotions after an act of violence.
