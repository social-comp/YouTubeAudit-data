## Data Description

YouTube audit data was collected during audit experiments---<i>Search</i> and <i>Watch</i> audits to examine YouTube's search and recommendation algorithms, respectively. The data is spread across four files. The description of each file along with their downloadable link is listed below.

**1. Queries file** 

filename: *queries.csv* [(download)](https://raw.githubusercontent.com/social-comp/YouTubeAudit-data/master/queries.csv)
   The file consists of a complete list of 49 search queries used in the audit study. It contains the following fields: -
   
  * ```ID:``` unique ID assigned to the search query
  * ```Topic:``` name of the misinformative search topic (9/11 conspiracy theories, chemtrail conspiracy theory, flat earth, moon landing conspiracy theories or vaccine controversies)
  * ```Seed Query:``` a collection of keywords representing the search topic
  * ```Query:``` search query name
  
   A snippet:
   
   <ID	Topic	Seed Query	Query 0	9/11 conspiracy theories	11-Sep	11-Sep>
   
      ```
{
  "firstName": "John",
  "lastName": "Smith",
  "age": 25
}
```
**2. Annotation Files**

* filname: *all_results.csv* [(download)](https://github.com/social-comp/YouTubeAudit-data/blob/master/all_results.csv?raw=true)
The file contains a collection of 56,475 videos compiled to link the stance of the video (promoting, debunking or neutral) with the personalization attribute audited (age, gender, geolocation or watch-history). The file contains the following fields: -
   * ```qid:``` unique ID assigned to the search query
   * ```vid_url:``` YouTube video URL	
   * ```vid_title:``` title of the YouTube video
   * ```aria-label:``` aria-label of the YouTube video	
   * ```annotation stance:``` stance assigned to the video by the annotators. The annotations are based on 9-point annotation scale ranging from -1 to 7
   * ```normalized_annotation:``` 3-point normalized scores with values -1(Promoting) , 0 (Neutral) and 1 (Debunking).
   * ```age_group:``` age group set while creating the google account This field can take values 1 (<18yrs), 2 (18-34yrs), 3 (35-50yrs) and 4 (>50yrs)
   * ```gender:``` gender set while creating google account (male/female)
   * ```activity:``` audit experiment during which the video was collected (search/watch)
   * ```activity_type:``` personalization attribute audited (demographics/geolocation)
   * ```topic:``` name of the misinformative search topic
   * ```geolocation:``` geolocation where the experiment was performed
   * ```geo_temperature:``` type of geolocation (hot/cold)
   * ```component_name:``` YouTube component audited/collected (Top5,SearchResults or UpNext)
   * ```order```	
   * ```vid_order```


* filename: *uniqueResults.csv* [(download)](https://github.com/social-comp/YouTubeAudit-data/blob/master/uniqueResults.csv?raw=true)
The file contains a list of 2,943 unique videos along with their annotation values. It contains the following fields: -
   * ```topic:```	misinformative search topic 
   * ```aria-label:``` aria-label of the YouTube video
   * ```description:``` description of the YouTube video
   * ```vid_title:``` title of the YouTube video
   * ```vid_url:``` URL of the YouTube video
   * ```annotation:``` same as (2)
   * ```normalized_annotation:``` same as (2)
   * ```duration:``` duration of the YouTube video
   * ```viewCount:``` view count of the YouTube video
   * ```likeCount:``` like count of the YouTube video
   * ```dislikeCount:``` dislike of the YouTube video
   * ```favoriteCount:``` favorite count of the YouTube video
   * ```commentCount:``` comment count of the YouTube video
   * ```popularity:``` popularity metric value of the YouTube video

A snippet:

```topic	aria-label	description	vid_title	vid_url	annotation	notes	normalized_annotation	duration	viewCount	likeCount	dislikeCount	favoriteCount	commentCount	popularity```
```911	Haunting, never-before-seen images of Ground Zero by CBS 7 years ago 3 minutes, 57 seconds 2,385,714 views	A few days after 9/11, FEMA sent its own cameras down into the ruins of the World Trade Center, filming for over 8 months and getting images no one else was able to get. CBS News justice and homeland security correspondent Bob Orr reports.	Haunting, never-before-seen images of Ground Zero	https://www.youtube.com/watch?v=coqYraFn-B4	0		0	237	2396779	8366	718	0	2649	2408512```


**3. Popularity Metric Files**

foldername: *popularity_metric.zip* [(download)](https://github.com/social-comp/YouTubeAudit-data/blob/master/popularity_metric.zip?raw=true)
This folder consists of 15 files (5 misinformative topics X 3 misinformative stance). Each file consists of the videos that were used to create watch histories of Google accounts for our watch experiments. We also provide video metadata (duration, view count, like count, dislike count, favorite count and comment count) as well as populatity metric values for these videos.



**4. SERP-MS scores** 

filename: *all_Top10_SERP-MM.csv* [(download)](https://raw.githubusercontent.com/social-comp/YouTubeAudit-data/master/all_Top10_SERP-MM.csv)
SERP-MS scores (SERP Misinformation Score) of the search engine results page retrieved during the audit experiments. The file contains the following fields: -
   * ```qid:``` unique ID assigned to the search query
   * ```query:``` search query name	
   * ```query_stance:``` stance assigned to the search query. It can take 3 valuues namely, -1(Promoting) , 0 (Neutral) and 1 (Debunking)
   * ```topic:``` name of the misinformative search topic
   * ```age_group:``` age group set while creating the google account
   * ```gender:``` gender set while creating google account (male/female)
   * ```activity:``` audit experiment during which the video was collected (search/watch)
   * ```activity_type:``` personalization attribute audited (demographics/geolocation)
   * ```stance:``` stance assigned to the video by the annotators. The annotations are based on 9-point annotation scale ranging from -1 to 7
   * ```geolocation:``` geolocation where the experiment was performed
   * ```geo_temperature:``` type of geolocation (hot/cold)
   * ```normalized_smm:``` SERP-MM score of the SERP

## Citation Information

If you use the dataset in your research, please cite the following paper:
> Eslam Hussein*, Prerna Juneja*, Tanushree Mitra. "Measuring Misinformation in Video Search Platforms: An Audit Study on YouTube". The 23rd ACM Conference on Computer-Supported Cooperative Work and Social Computing. 2020.





