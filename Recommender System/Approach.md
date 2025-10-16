Summary: The solution/practices of industry on recommender systems.

Amazon.com: 
- Recommendations are split into "buy again", "customers who bought this also bought".
- Recommendations also ranging on general towards personalized.
- Recommenders: [[Hybrid Recommender Systems]] (with [[Content-based Recommender Systems]] & [[Collaborative Filtering]] & [[Popularity-Based Recommender]] & [[Contextual Recommender]]).

Zagat: 
- Aggregates restaurant ratings form various individuals scoring from food, decor, and services on scale 0 to 30. Turn it into statistics which used for [[Non-Personalized Recommendations]].
- Recommenders: [[Non-Personalized Recommendations]] based on summary statistics. Which leans toward community opinions than each users.

Conde Nast Traveler: 
- Uses [[Non-Personalized Recommendations]] based on percentage-based scoring. They ask for user to rates the hotels, cruise lines, and other service as "poor," "fair," "good," "very good," or "excellent." which can be turn back into numbers but this also good enough.
- Uses only the "good" and "very good" percentage as score for that service.
- Focus mainly on customer that are satisfied by the service. (May lead to bias but good intension on helping the service to stay alive).

Reddit: 
- Uses a voting system for users to update or downvote posts, which directly influence the visibility of the content. The net upvotes determine the popularity of a post (upvote - downvote).
- Ranking algorithm: Newer posts have higher chance to be viewed as the old post gradually lost visibility. As the system has a time decay factor which will out growth the popularity mention above.
- Recommenders: [[Non-Personalized Recommendations]] base on voting system.