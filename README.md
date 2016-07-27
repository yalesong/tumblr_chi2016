nimated GIF Dataset (CHI 2016)
This repository contains the Tumblr animated GIF dataset used in our CHI 2016 paper **"Fast, Cheap, and Good: Why Animated GIFs Engage Us."** 

## Introduction
We crawled the entire animated GIF posts created on Tumblr between July 2014 and January 2015. Since our goal is to study what makes an animated GIF engaging, we used the following criteria when selecting the posts:

1. It was a photo post.
2. It contained one single animated GIF.
3. It was not marked Not Suitable for Work (NSFW).
4. It was originally created by the user, not reblogged from others.
5. Once posted, it had never been edited during the given time frame.

For each post, we collected the number of likes and reblogs within the same period of time. Likes and reblogs are social signals that are designed and used differently on Tumblr. Likes are lightweight signals that usually signify the users interest in content posted. Reblogs on the other hand are forms of sharing the content which requires more commitment from users. 

We performed stratified sampling on the crawled data, enabling us to generate a workable subset consisting of a randomized sample of approximately 25,000 posts from four different sections of the distribution, ranging from the most frequently liked and reblogged to the least frequently liked and reblogged. The resulting dataset contains 99,844 posts. 

## The Data
`tumblr_chi2016.tsv` is a tab-separated values (TSV) format file, containing 99,844 animated GIFs and their social engagement measures: the number of likes and the number of reblogs. The first column contains public URLs to download the GIFs, the second and the third contain the number of likes and the nubmer of reblogs, respectively. The last column is the sum of the two (#likes and #reblogs). 

`features.csv` and `features_fieldnames.csv` are comma-separated values (CSV) format files, containing the features we computed for analyzing the engagement of animated GIFs. See our CHI 2016 paper for detailed descriptions about the features.

## Reference
Saeideh Bakhshi, David Shamma, Lyndon Kennedy, Yale Song, Paloma de Juan, Joseph 'Jofish' Kaye. **"Fast, Cheap, and Good: Why Animated GIFs Engage Us.** In Proceedings of the 2016 CHI Conference on Human Factors in Computing Systems (CHI 2016), San Jose, CA, USA, May 7-12, 2016.
