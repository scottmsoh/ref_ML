
## tunning methods

1. Concepts to choose: User vs Item-based
2. Similarity metrics: cosine, Pearson,  Jaccard, and etc)
3. Number of K

4. Handle Sparse dataset: missing values
5. Normalize: 1~5 scale -> 0~1 conversion (quantity will be much huge)
6. Cold start: content-based filtering

7. Weighted KNN: closer neighbors impact more 
8. Temporal dynamics: time-based, weighted more on recent data (most_recent_date - df['time-stamp']</br>
   (Able to control tendency of weight from Decay_rate(decay_rate is getting smaller, time's weight can be much higher)</br>

![Image 2024-01-02 at 10 38 AM](https://github.com/scottmsoh/ref_ML/assets/112598791/2e3100b3-76d2-4778-8b1b-42af925dfd46)

9. Computing similarity between two users, give more weight to items that were both rated recently.</br>
10. Weekdays vs. weekends, or morning vs. evening.</br>
11. Temporal Cross-validation: train on earlier data and test on more recent data</br>
    to ensure the model performs well on current user preferences.</br>


    
