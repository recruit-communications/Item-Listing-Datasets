# Item-Listing Datasets

This repository contains datasets used and described in the paper[^1]:  

[^1]:https://www.frontiersin.org/articles/10.3389/fcomp.2019.00002

"Item Listing Optimization for E-commerce Websites Based on Diversity"  
Authors: N. Nishimura, K. Tanahashi, K. Suganuma, M. J. Miyama, M. Ohzeki.  
Journal: Frontiers in Computer Science  
DOI: 10.3389/fcomp.2019.00002  
Contact: Naoki Nishimura (nishimura@r.recruit.co.jp)  

This dataset contains popularity (bias) values and similarity (interaction) values for the top 10 accessed areas on the hotel reservation website Jalan[^2]. These values were estimated using the website's access log from the past six months, which includes the date and time the customer accessed the item list screen, the position of each item when the item list screen was accessed, and information about the hotel at which the customer made their reservation. 

[^2]:https://www.jalan.net/en/japan_hotels_ryokan/

If you use the datasets for your work, please consider citing the paper.

-----
Files:
-----

bias_area*_size**.csv: Popularity p_ij of the ** most accessed hotels in area *. p_ij is the estimated popularity of a hotel i ∈ I when it is placed in a position j ∈ J.

interaction_area*_size**.csv: Similarity f_ii' of the ** most accessed hotels in area *. f_ii' is the estimated similarity of the hotels pair i, i' ∈ I. f_ii' is calculated using the log of the number of items browsed during the same session.

interaction_area1_size8_semantic.csv: Similarity f_ii' of the 8 most accessed hotels in area 1. f_ii' is the estimated similarity of the hotels pair i, i' ∈ I. f_ii' is calculated using the two-dimensional vector of whether the area is north or south and whether the hotel is a city or budget hotel.

-----
Correspondence with paper notation:
-----

Areas X,Y,Z in Figure 3 and 4 correspond to areas 1, 2 and 3 in dataset respectively.  
The hotel symbols A to H in Figure 5 correspond to the hotel_ids in the table below.

| Hotel symbol | hotel_id |
|:-----------:|:------------:|
| A | fee6c0a8f3 |
| B | 0d26626dae |
| C | 5a18d4d461 |
| D | 7405978021 |
| E | 80bdccbfe5 |
| F | bdba2530bd |
| G | d91db6f9c9 |
| H | 7fced5b857 |
