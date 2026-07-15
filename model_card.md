# 🎧 Model Card: Music Recommender Simulation

## 1. Model Name

VibeFinder 1.0

---

## 2. Goal / Task

This recommender suggests songs that fit a user’s taste. It tries to predict which songs a person would likely enjoy based on simple preferences like genre, mood, and energy.

---

## 3. Data Used

The system uses a small dataset with 10 songs. Each song has features such as genre, mood, energy, tempo, valence, danceability, and acousticness. The dataset is small, so it does not cover every style or mood.

---

## 4. Algorithm Summary

The system gives points when a song matches the user’s favorite genre and mood. It also checks how close the song’s energy is to the user’s target energy. If the user likes acoustic songs, that gives the song a small extra boost. The songs are ranked from highest score to lowest.

---

## 5. Observed Behavior / Biases

The system often favors easy matches. For example, “Gym Hero” shows up often for happy pop profiles because it fits several simple signals at once. This can make the recommendations feel reasonable, but it can also make the system look too narrow or too repetitive.

---

## 6. Evaluation Process

I tested the recommender with several user profiles. I used a default happy pop profile, a conflicting profile, an acoustic profile, a genre mismatch profile, and an extreme energy profile. I compared the top results and checked whether the rankings made sense. I also tried changing the weights to see how sensitive the system was.

---

## 7. Intended Use and Non-Intended Use

This system is meant for learning and small experiments in recommender design. It is not meant for real music streaming decisions or for making important choices about a person’s taste.

---

## 8. Ideas for Improvement

- Add more songs and more genres.
- Add more balanced features so the system does not rely so much on genre.
- Make the scoring more flexible so it can handle mixed or unusual tastes better.

---

## 9. Strengths

The system works well when the user has clear and simple preferences. It gives sensible results for profiles that are easy to describe, such as happy pop or acoustic mood.

---

## 10. Limitations and Bias

The system can overvalue obvious features like genre or energy. It may miss better matches that are less obvious. It also reflects the limits of a small dataset.

---

## 11. Evaluation

The evaluation section above shows that the system changes its output when the user profile changes. That is a good sign. It also shows that the system can be influenced too strongly by a few simple signals.

---

## 12. Future Work

I would like to add more songs, more user profiles, and a better scoring method. I would also like to make the recommendations more diverse and easier to explain.

---

## 13. Personal Reflection

My biggest learning moment was seeing how a small scoring rule can make a recommender feel smart even when it is very simple. I also learned that a few clear signals, like genre and energy, can shape the results more than I first expected.

Using AI tools helped me move faster. They were useful for writing code, testing ideas, and explaining the ranking logic. I still had to double-check the results, especially when the output looked surprising or when the weights changed, because the system can be wrong even when the code looks correct.

I was surprised that a simple algorithm could still feel like a real recommendation system. The output seemed believable because it matched obvious patterns, even though the logic was basic. If I extended this project, I would add more songs, more features, and a better way to balance genre, mood, and energy so the recommendations feel more diverse and less repetitive.

