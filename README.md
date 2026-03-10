# Customer Acquisition Markov Attribution Engine

## Overview
This project analyzes multi-channel customer journeys to determine how different marketing channels contribute to customer conversions.  
A **Markov Chain Attribution Model** is used to calculate the contribution of each marketing channel by measuring the *removal effect*.

This approach helps businesses optimize marketing spend by identifying the channels that drive the most value in the customer acquisition funnel.

---

## Dataset
Source: Kaggle – Multi-Touch Marketing Attribution Dataset

The dataset contains user interaction logs across multiple marketing channels including:

- Email
- Social Media
- Search Ads
- Display Ads
- Direct Traffic
- Referral

Each record represents a marketing interaction with fields including:

| Column | Description |
|------|-------------|
| User ID | Unique customer identifier |
| Timestamp | Interaction time |
| Channel | Marketing channel |
| Campaign | Campaign name |
| Conversion | Whether the interaction led to conversion |

---

## Methodology

The analysis follows these steps:

1. **Customer Journey Reconstruction**  
   Rebuilt each user's interaction path using chronological ordering of events.

2. **Transition Matrix Construction**  
   Calculated transition probabilities between marketing channels.

3. **Markov Chain Modeling**  
   Built a Markov model to represent channel transitions in the customer journey.

4. **Removal Effect Calculation**  
   Simulated removal of each channel to measure its impact on overall conversion probability.

5. **Channel Attribution Analysis**  
   Normalized removal effects to estimate each channel’s contribution.

---

## Results

The Markov attribution model reveals the relative importance of marketing channels in driving conversions.

Example findings:

- Referral channels showed strong downstream conversion influence.
- Social media contributed significantly during the early awareness stage.
- Direct traffic frequently acted as the final conversion channel.

These insights can guide **marketing budget optimization and channel strategy**.

---

## Visualization

Channel contribution visualization:

![Channel Attribution](visuals/channel_contribution.png)

---

## Tech Stack

- Python
- Pandas
- NumPy
- Matplotlib
- Markov Chain modeling

---


---

## Key Business Insight

Marketing attribution analysis suggests that reallocating marketing budget toward high-impact channels can significantly improve conversion efficiency.

Understanding the full customer journey provides more accurate attribution compared to traditional last-touch models.

---

## Future Improvements

- Compare Markov attribution with **Last-touch and First-touch models**
- Build a **dashboard for marketing channel performance**
- Implement **Monte Carlo simulations for channel removal analysis**

---

## Author

Valasapalli Sai Shanth Kumar  
