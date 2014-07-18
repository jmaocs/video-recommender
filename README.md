video_recommendation
====================

This includes three files

* video_tag_fetch.py

		- fetch the tags (show name, Genre, Type) for each video given the keywords extracted from the description and title of the corresponding video
		- fetch the tag (actors) from the extracted keywords if it is a actor or actress 's name based on dbpedia
* assign_tag.py

		- assign all the fetched tags to each video and output the results as tagged_videos.json
* calc_sim.py

		- calculate the total similarity score for any two videos based on the similarity score of actors, show name, and TFIDF score 
		- output three related videos for each video into recommended_videos.txt
   
Dependency

* The required dependency is Numpy

To run the program

* python assign_tag.py
* python calc_sim.py > recommended_videos.txt