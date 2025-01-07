# ShampYou: A Personalized Shampoo Recommender

Personalized shampoo recommendation system leveraging user reviews and price data to help consumers find the best product tailored to their preferences. Analysis conducted using web-scraped data from **Influenster.com** and **Ebay.com**.

---

## **Overview**
Finding the perfect shampoo can be overwhelming, with over 22,000 products available on platforms like Influenster. ShampYou aims to simplify this decision-making process by:
- Analyzing customer reviews for popular attributes like "soft," "silky," or "frizz-free."
- Recommending affordable and high-quality alternatives.
- Supporting product exploration beyond just popularity.

---
**Data Collection**:
   - Scraped reviews and ratings for the top 100 shampoos.
   - Fuzzy-matched price data from Ebay to enhance recommendations.

**Analysis Process**:
   - **Review Translation**: Translated foreign language reviews into English.
   - **Word Frequency**: Analyzed frequently mentioned attributes (e.g., "hydration," "volume").
   - **Cosine Similarity**: Measured similarity between products based on review attributes.
   - **spaCy Similarity**: Used spaCy for additional product similarity computation.
   - **Sentiment Analysis**: Applied Vader sentiment analysis to compute an overall score.

**Output**:
   - **Attribute-Based Profiles**: Recommendations tailored to user preferences, such as:
     - Soft, silky, and shiny.
     - Frizz-free and affordable.
     - Curly and nourishing.
     - Herbal and hydrating.
   - **Substitute Suggestions**: Similar products recommended based on an existing favorite shampoo.

---

## **Example Output**
### **User's Desired Shampoo Attributes:** Soft, Shiny, Silky
| Product Recommendation Based on Cosine Similarity  | Price   |
|----------------------------------------------------|---------|
| Suave Moroccan Infusion Shine Shampoo              | $4.43   |
| Pantene Pro-V Ultimate 10 Shampoo                  | $7.01   |
| Herbal Essences Argan Oil of Morocco Shampoo       | $10.95  |

---
