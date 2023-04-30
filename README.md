# Twitter Analysis
INTRODUCTION
Mass shootings are a serious and ongoing issue in many countries, and they often lead to heated debates and discussions around gun control measures. That's why we decided to analyse one specific shooting, the one that unfortunately happened in Nashville, Tennessee on the last 27th of March of the current year 2023; specifically in the Covenant school.

This event went viral on social media platforms, like Twitter, which actually offers an opportunity to examine these discussions and to gain insight into public opinion on the matter. In this project we conducted an analysis on Twitter using hashtags to identify how people were talking about the Covenant school shooting. 

We also applied the Louvain Method, which is a community detection algorithm that uses modularity optimization to identify clusters or communities in networks.Thus, we used it in order to identify clusters of tweets that are predominantly Pro or Anti-gun control with the goal of seeing if there is any polarization in public opinion

ANALYSIS 

The results of the Louvain method does not show a direct polarization of opinions but rather a collection of different clusters. Some of these clusters lean towards a pro or anti gun stance while others clusters have no poitical opinions yet other themes can still be identified within them. 

Notably, even the political clusters are not entierley unanimous in their leaning and have hashtags within them that seem misplaced in relation to the general sentiments of the hashtags in that cluster. This may however be due to tweets which support one opinion but point to the hypocrisy of other opinions or use the hashtags of these other opinions ironically.

![SNA Final group project-1](https://user-images.githubusercontent.com/130977434/235372823-53755950-5a2b-4ec5-bd60-80c3f4cb8df5.png)


RED: One of the more prominent hashtags: 
#guncontrol, #guncontrolnow, #enoughisenough, #stopmassshooting, #assultweaponban, #secureourschools, #gundlawssavelives

#goplovesgunsmorethanourkids, #gopdoesnotcareifkidsdie, #gopisnottheprolifepartytheyareprodgundeath these all refer to the grand old part, synonymous with the republican party. As this cluster also has hashtags which encourage gun control and ban of weapons, one can assume that those who tend to be critical of the republican party will also be for gun laws. This will often be those who vote democrat due to americas two party system.

#prolife seems odd in the context but may be calling out hypocrisies of republicans who will often make prolife arguments in relation to abortion but not in relation to guncontrol. 



BLUE: is also a more political cluster with different views to the red one. 
#tstandsforterrorist, #genderdysphoriaisanillness, #redflagtrans, #2ashallnotbeinfinged, #timburchette, #backtheblue, #transgenderproblems, #notthegunsfault
#liberalsmustgo, #liberalhypocrisy,#liberalismisacult, #liberalismisamentaldisorder, #democratsaredestroyingamerica This cluster is typically pro gun and anti liberal which opposes the red cluster. 
 #genderaffrimingcare and #mentalhealthawareness again seem out of place in the context of the other blue tweets but we cannot tell the context of these tweets and thereby cannot be sure if they align with the opinions of the cluster or not. 



GREEN: is also political and typically pro gun control and critiques of the republican party. 
#anothershooting, #itsthegunsandtherepublicans, #banar15s, #stop, #gopdomesticterrorists, #saveourchildren, #gunsafteynow, #yourchildcouldbenext
#itsthegunsstupid which seems to be a direct response to the hashtag from thew blue cluster #notthegunsfault



TURQUOISE: does not seem to have a political leaning or stance on gun voilence but is more about themes of religion and charity. Notably, not just christianity is mentioned. 
#bible, #pray, #christian, #jesusislord, #ramadan, #jesus, #christianity, #givingtuesday



PURPLE: contains a range of hastags but many of them are references to other shootings that have occurred.
#buffalomassacre, #parklandmassacre, #virginashooting, #columbine, #elpasoshooting, #dadeville, #sandyhook


Some clusters have seeminly nothing to do with the theme of gunvoilence but concern other relevant topics such as #nft or #ukraine. This may be linked to social media culture and an attempt to gain exposure through trending hashtags despite their relevance to the topic of the tweet. 







CONCLUSION


In conclusion, this analysis can’t show polarization but helps us to identify how people are talking about a recent mass shooting. To do so, we use the Louvain community iGraph algorithm that allows us to identify clusters with mostly pro-gun control tweets and to some extent anti-gun control tweets.

To further analyze our results, we compare them to existing surveys which were made by experts using machine learning to analyze reactions on Twitter about the Sandy Hook Elementary school shooting (Wang, N., Varghese, B., & Donnelly, P. (2017). A Machine Learning Analysis of Twitter Sentiment to the Sandy Hook Shootings. ) We can notice the recurrences of some hashtags on Twitter after a mass shooting like #PrayFor  or #guncontrol  that builds a social media culture that automatically give people some conventions while expressing their emotions after an act of violence.
