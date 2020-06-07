# Recommendation-implicit_feedback

There is two kind of feedbacks when we gain data for Recommendation purpose.
Explicit feedback is like ratings on the movie. User explicitly rate the item, so we can easily know whether user liked it or not.
Implicit feedback is diverse action of the user on the item. When user hear the music, he can hear only half of it. Also we can't know wheter he like it or not. Also, in the online shopping, user can 'view' the item, or 'add to shopping cart", or 'buy the item', etc. From the implicit feedback, user didn't explicitly rate the item, so it could be harder to analysis the data and give the recommend

To implement recommendataion for the implicit feedback, there are several methods.
Model is form the paper
[ Collaborative Filtering for Implicit Feedback Datasets](http://yifanhu.net/PUB/cf.pdf)
and I followed the method which is called ALS(Alternating Least Square) in the paper of 
[Applications of the Conjugate Gradient Method for Implicit Feedback Collaborative Filtering](https://www.semanticscholar.org/paper/Applications-of-the-conjugate-gradient-method-for-Tak%C3%A1cs-Pil%C3%A1szy/bfdf7af6cf7fd7bb5e6b6db5bbd91be11597eaf0)
which speed-up the ALS method.

For the testing, I used the 
[lastfm dataset](http://ocelma.net/MusicRecommendationDataset/lastfm-360K.html)
containing the listening behaviour of 360,000 users. It contains the user id, an artist id, the name of the artists and the number of times a user played any given artist.
