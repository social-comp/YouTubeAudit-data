## Data Description

YouTube audit data was collected during audit experiments---<i>Search</i> and <i>Watch</i> audits to examine YouTube's search and recommendation algorithms, respectively. The data is spread accross five files. The description of each file along with their downloadable link is listed below.

**1. Queries file** 

filename: *queries.xlsx* [(download)](https://github.com/social-comp/YouTubeAudit-data/blob/master/queries.xlsx?raw=true)
   The file consists of a complete list of 49 search queries used in the audit study. It contains the following fields: -
   
   * *ID:* unique ID assigned to the search query
   * *Topic:* name of the misinformative search topic (9/11 conspiracy theories, chemtrail conspiracy theory, flat earth, moon landing conspiracy theories or vaccine controversies)
   * *Seed Query:* a collection of keywords representing the search topic
   * *Query:* search query name
   
**2. Annotation Files**

* filname: *all_results.xlsx* [(download)](https://github.com/social-comp/YouTubeAudit-data/blob/master/all_results.xlsx?raw=true)
The file contains a collection of 56,475 videos compiled to link the stance of the video (promoting, debunking or neutral) with the personalization attribute audited (age, gender, geolocation or watch-history). The file contains the following fields: -
   * qid: unique ID assigned to the search query
   * vid_url: YouTube video URL	
   * vid_title: title of the YouTube video
   * aria-label: aria-label of the YouTube video	
   * annotation stance: stance assigned to the video by the annotators. The annotations are based on 9-point annotation scale ranging from -1 to 7
   * normalized_annotation: 3-point normalized scores with values -1(Promoting) , 0 (Neutral) and 1 (Debunking).
   * age_group: age set while creating the google account
   * gender: gender set while creating google account (male/female)
   * activity	
   * activity_type	
   * topic	
   * geolocation	
   * geo_temperature	
   * component_name	
   * order	
   * vid_order


* filename: *uniqueResults.xlsx* [(download)](https://github.com/social-comp/YouTubeAudit-data/blob/master/uniqueResults.csv?raw=true)
The file contains a list of 2,943 unique videos along with their annotation values.

**3. Popularity Metric Files**

filename: *popularity metric.zip* [(download)](https://github.com/social-comp/YouTubeAudit-data/blob/master/popularity_metric.zip?raw=true)
This folder consists of 15 files (5 misinformative topics X 3 misinformative stance). Each file consists of the videos that were used to create watch histories of Google accounts for our watch experiments. We also provide video metadata (duration, view count, like count, dislike count, favorite count and comment count) as well as populatity metric values for these videos.



**4. SERP-MS scores** 

filename: *all_Top10_SERP-MM* [(download)](https://github.com/social-comp/YouTubeAudit-data/blob/master/all_Top10_SERP-MM.xlsx?raw=true)
SERP-MS scores (SERP Misinformation Score) of the search engine results page retrieved during the audit experiments. The file contains the following fields: -
   * qid: unique ID assigned to the search query
   * query: search query name	
   * query_stance	
   * topic	
   * age_group	
   * gender	
   * activity	
   * activity_type	
   * stance	
   * geolocation	
   * geo_temperature	
   * normalized_smm







