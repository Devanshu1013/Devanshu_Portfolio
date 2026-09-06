<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=rect&color=0:0A2647,100:205295&height=180&section=header&text=Movies%20Recommendation%20System&fontSize=32&fontColor=FFFFFF&fontAlignY=40&desc=Comparing%20Content-Based%2C%20Collaborative%2C%20and%20Hybrid%20Approaches&descSize=16&descAlignY=65" width="100%"/>
</p>

<p align="center">
🔗 <a href="https://github.com/Devanshu1013/Movies-Recommendation">Original Repository</a> &nbsp;|&nbsp; <a href="https://github.com/Devanshu1013/Devanshu_Portfolio/blob/main/README.md">← Back to Portfolio</a>
</p>

---

## Overview

A DS8001 course project comparing multiple recommendation strategies — content-based, collaborative filtering, popularity-based, hybrid, and SVD — using real-world movie data from Kaggle, with a focus on evaluating each approach's strengths and trade-offs.

**Highlights:**
- Compares 5 different recommendation strategies on the same dataset
- Includes matrix factorization (SVD) alongside classic collaborative and content-based methods
- Evaluation-driven approach to compare recommendation quality across models

## Approaches & Results

**Popularity-Based** ranks movies purely by volume and audience reach, giving a simple, non-personalized baseline.

<p align="center">
  <img src="assets/movies-popularity.png" alt="Top 10 most popular movies" width="60%"/>
</p>

**Content-Based Filtering** recommends movies with similar attributes (genre, cast, keywords) using cosine similarity over TF-IDF and CountVectorizer representations. For a query like *Hulk*, both vectorizers surface genre-aligned titles such as *The Incredible Hulk* and *Fantastic Four*, with similarity scores in a comparable range.

<p align="center">
  <img src="assets/movies-content-based.png" alt="Top content-based recommendations for 'Hulk'" width="65%"/>
</p>

**Collaborative Filtering** predicts ratings from user behavior patterns rather than movie attributes. User–user and item–item variants were both evaluated on RMSE, with user–user CF (3.34) slightly outperforming item–item CF (3.47).

<p align="center">
  <img src="assets/movies-collaborative.png" alt="RMSE comparison of user-user vs item-item collaborative filtering" width="55%"/>
</p>

**Hybrid Model** blends popularity with weighted average ratings to balance broad appeal against genuine audience reception — surfacing titles like *Pulp Fiction*, *The Dark Knight*, and *The Shawshank Redemption* alongside high-popularity picks.

<p align="center">
  <img src="assets/movies-hybrid-top10.png" alt="Top 10 movies by popularity and weighted average" width="60%"/>
</p>

A further comparison of blending strategies shows the weighted-average approach (RMSE 5.40) edging out the blended score method (RMSE 5.50) on this dataset.

<p align="center">
  <img src="assets/movies-hybrid-rmse.png" alt="RMSE comparison of weighted average vs blended score" width="55%"/>
</p>

## Tech Stack

`Python` `Pandas` `Scikit-learn` `SVD` `Collaborative Filtering`

---

<p align="center">
<a href="https://github.com/Devanshu1013/Devanshu_Portfolio/blob/main/README.md">← Back to Portfolio</a> &nbsp;|&nbsp; 🔗 <a href="https://github.com/Devanshu1013/Movies-Recommendation">View on GitHub</a>
</p>
