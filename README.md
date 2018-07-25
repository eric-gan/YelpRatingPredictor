# Yelp Rating Predictor

A visualization of restaurant ratings using an unsupervised machine learning model through k-means clustering and the Yelp academic dataset. In this visualization, Berkeley is segmented into regions, where each region is shaded by the predicted rating of the closest restaurant (yellow is 5 stars, blue is 1 star). Specifically, the visualization constructed is a Voronoi diagram.

##How to run:

Download and navigate to the corresponding folder. Then

1. In the `users` directory, you'll see a couple of `.dat` files. Copy one of them and rename the new file to `yourname.dat` (for example, `john.dat`).

2. In the new file (e.g. `john.dat`), you'll see something like the following:

```
make_user(
    'John Appleseed',   # name
    [                   # reviews
        make_review('Jasmine Thai', 4.0),
        ...
    ]
```

Replace the second line with your name (as a string).

3. Replace the existing reviews with reviews of your own! You can get a list of Berkeley restaurants with the following command: `python3 recommend.py -r`

Rate a couple of your favorite (or least favorite) restaurants.

4. Use `recommend.py` to predict ratings for you: `python3 recommend.py -u john -k 2 -p -q Sandwiches`

(Replace john with your name.) Clusters are adjusted using (the -k option) and queries using (the -q option).

Technologies Used: Python, JavaScript, HTML
