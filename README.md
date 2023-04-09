# SoMeOptimumPost

Final project for the Building AI course

## Summary

Describe briefly in 2-3 sentences what your project is about. About 250 characters is a nice length! 


## Background
When making a post on social media, it is often hard to know what reach it will have and how large impact it will have on those reading it. Since making posts can require some effort, it would be helpful to get an indication of how large impact a planned post might have. Personally, this would make it easier to know when to expend efforts on for example sharing a petition or an opportunity, as well as choose which social media platforms I might make such a post on. Since I am engaged in environmental issues, such help might give my posts a wider reach and make them easier to take seriously.


## How is it used?
My idea for an AI method should be used both before and after making a post on a given social media platform. Before making a post, one would enter relevant information about the post one is about to share, in particular the text to be shared. Then, the AI method would return a score for how large impact the post can be expected to have, mainly based on number of views and/or likes, as well as expected number of people who will for example open a link shared in the post. This makes it easier for you to make the decision whether to make the post or not, and whether to rewrite it a bit, for example.

After the post has been made, the AI method would collect data related to the impact of the post, for example number of views and/or likes, as well as number of people who have opened a given link shared in the post. Ideally, it would be possible to access this data in a transparent and understandable manner for the user and others. Also, the user might be able to check a box if they would like the data that the method collects about their post to be possible to use when judging the impact of others' posts. The data thus collected would serve as additional data to use for judging the expected impact of future posts.

The use of data from one's own previous posts should be separated from the use of data from others' posts, for example by giving a main score based on only one's own previous posts and in addition supplying a score framed as "Others would get this impact score if making this post: ". The reason for this separation is that it is hard to quantitatively compare one's own posts with those of others, who might have another number of followers or focus on other social media platforms.

The method should feel easy and safe to use for essentially anyone.


## Data sources and AI methods
The data used comes from both one's previous posts, but also the posts of other consenting users. However, the data of others should remain anonymous even if it is allowed to use it.

To compare the drafted post to previous posts, the focus would probably be on the text in the post. In this context, use of Natural Language Processing (NLP) would probably be useful. To assign an expected impact score to the post, a classification based on the k nearest neighbours can likely be done, possibly by calculating the mean of their k respective data points and calculating the score based on this.


## Challenges
Predicting the impact of a written text is very complex, even for a human possessing all the information that the AI method would. There are a lot of indicators which might be relevant for the impact of a post, such as the length of the text, frequency of the words (maybe quantified by TF-IDF scores) and time of day for the post. Therefore, it is probably a challenge to choose which indicators to include, and which to leave out, in order to make the computational cost bearable and make the results of the AI method transparent for those who want to investigate potential biases etc.

An ethical concern is what data might be used by the AI method. For one, it might be hard to get informed consent regarding all different types of data that the method will use, since being familiar with all those different kinds of data might require extensive knowledge. It is also possible to change one's mind regarding what data one wishes to share with the method, especially the data which is used also for others' posts. However, it might be hard to remember which kinds of data were included in the initial consent given to use one's data. Such privacy concerns are somewhat addressed by having to make an active choice to share any data, but those concerns arguably remain to some extent.


## What next?
Since the AI method is dependent on quite large quantities of data, an important first step is mapping the different sources of relevant data that exist today, as a means to ensure that there will be at least some data to base the predictions on before the method has gathered a sizeable amount of data by itself.

It would also be important to enlist the help of people with expertise in the ethics of data consent and the use of personal data by an AI method.

Finally, there are many ways to extend the AI method if it is implemented. For example, it might be possible to specify the goal one has when making a post, eg getting as many people as possible to share a petition or inspiring those reading to get in touch regarding the subject matter of the post. It might also be possible to use certain labels for the posts, such as "petition" or "sharing best practices". Both of the above extensions might make it possible to get an impact score better tailored to the purpose of the post.


## Acknowledgments
Thanks to the people behind the "Introduction to AI" and "Building AI" courses for lucid learning about different aspects of AI!
