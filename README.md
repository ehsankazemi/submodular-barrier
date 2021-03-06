# Submodular Maximization Through Barrier Functions

The code accompanying the paper entitled "Submodular Maximization Through Barrier Functions"

1. utility_functions.py contains the data loaders, constraints and functions.
	a. get_video_data() loads the data for video summarizing application.
	b. get_graph_data() loads netwokrs and community assignments.
	c. loadTwitterData() loads the twitter datasets.
	d. get_movie_recommendation_data() 
	e. get_yelp_data() loads the yelp dataset with the distance of each location to each POI.

2. algorithms.py contains the submodular maximization algorithms we use.

3. video_summarization_application.py: 
	a. This script provides an instance of running our implemented algorithms on a real-world application.
	b. Our objective is to select a subset of frames from these videos in order to maximize a utility function f(S) (which represents the diversity of frames). We set limits for the maximum num- ber of allowed frames from each video (referred to as mi), where we consider the same value of mi for all five videos. We also want to bound the total entropy of the selection as a proxy for the storage size of the selected summary.
	c. We compare the performance of our proposed algorithms with several baselines. Our first baseline is the vanilla Greedy algorithm. Our second baseline is Density Greedy. We also consider the state-of-the-art algorithm (called Fast) for maximizing monotone and submodular functions under a k matroid constraints and l knapsack constraints (Badanidiyuru & Vondrak, 2014). 

4. All the datasets we have used are provided in the "datasets" directory.
