

```Python

import pandas as pd
import numpy as np

# Example DataFrame
ratings_df = pd.DataFrame({
    'user_id': [1, 1, 2, 2],
    'movie_id': [101, 102, 101, 103],
    'rating': [4, 3, 5, 2],
    'timestamp': [10, 20, 15, 5]  # Days ago the rating was given
})

# Current day for the sake of example
current_day = 20  # Assume this is the current day in the same time unit as the timestamp

# Decay rate
lambda_decay = 0.1

# Calculate time since each rating
ratings_df['days_since_rating'] = current_day - ratings_df['timestamp']

# Apply exponential decay to ratings
ratings_df['decay_factor'] = np.exp(-lambda_decay * ratings_df['days_since_rating'])
ratings_df['weighted_rating'] = ratings_df['rating'] * ratings_df['decay_factor']

print(ratings_df)

```
