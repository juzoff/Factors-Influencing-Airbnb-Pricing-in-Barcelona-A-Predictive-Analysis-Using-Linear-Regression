# Branch 6: Final Insights & Analysis

### > FILE: 
    - Credit Score - Prediction, Scoring and Implementation.sas
    - New_Data.csv
    - scored_new_data_creditscore.csv

## •	Insights From FInal Linear Model
### Top 5 Positive Influencers on Target Variable - Price
- ![image](https://github.com/user-attachments/assets/04ace788-73e5-47c0-8906-78d60d15c7fb)

    - property_typeNature.lodge - $4,856.29
         - Premium Pricing: Lodge-type properties significantly command higher prices, suggesting unique features and experiences attract guests willing to pay more.
         - Desirability Factors: Their appeal likely stems from location and amenities, making them attractive investments for developers.
         - Marketing Leverage: Highlighting the distinctive nature of lodges can enhance occupancy rates and justify premium pricing.
    - host_neighbourhoodCoral.Gables - $1,490.38
         - Neighborhood Value: Properties in Coral Gables show enhanced pricing due to its desirability, amenities, and community appeal.
         - Attractiveness: Strong demographics and community characteristics contribute to higher rental rates.
         - Promotional Opportunities: Marketing should emphasize the benefits of staying in this neighborhood to attract potential guests.
    - host_response_rate48 - $889.66
         - Bimodal Pricing Dynamics: Moderate response rates correlate with higher prices, while higher rates (e.g., 70-90%) lead to lower estimates, possibly indicating competitive pricing strategies.
         - Value Proposition: Higher pricing may suggest unique offerings or quality experiences rather than just responsiveness.
         - Guest Preferences: Guests may appreciate a balanced approach to service, where personalized attention is more valued than sheer volume of responses.
    - host_neighbourhoodLa.Latina - $869.30
         - Cultural Appeal: Properties in La Latina can attain higher prices due to cultural attractions and vibrant community life.
         - Local Amenities: The neighborhood might offer compelling reasons for guests to pay more, such as nightlife and historical significance.
         - Tailored Marketing: Highlighting neighborhood-specific attractions can enhance appeal and pricing strategies.
    - Gym_binary - $308.56
         - Impact of Amenities: While lower in comparison, gym access adds value, reflecting a growing trend toward health-conscious travel.
         - Market Differentiation: Properties with gyms can attract fitness-focused guests, supporting higher price points.
         - Niche Targeting: Focused marketing towards health-oriented travelers can further enhance property appeal.


### Top 5 Negative Influencers on Target Variable - Price
- ![image](https://github.com/user-attachments/assets/3cd8b8b2-b0c6-483c-ab8b-997125513a75)

    - host_is_superhost (Estimate: -10.69)
      - Interpretation: This attribute indicates whether the host is a superhost. Since the value is 'f' (false), it suggests that the property is not managed by a superhost, which correlates with a negative impact on price. Superhosts are typically recognized for providing exceptional service and experiences, so listings without this designation may command lower prices.

    - host_response_rate61 (Estimate: -25.41)
      - Interpretation: A response rate of 61% suggests that the host is not very responsive to inquiries. Low responsiveness can deter potential guests, directly affecting the appeal and booking rate of the listing, hence a reduction in price.

    - host_neighbourhoodAdelfas (Estimate: -32.25)
      - Interpretation: The listing is located in the Adelfas neighborhood, which has a significant negative impact on price. This could indicate that Adelfas is perceived as less desirable compared to other neighborhoods in the dataset, possibly due to factors like amenities, safety, and attractiveness.

    - host_response_rate72 (Estimate: -51.15)
      - Interpretation: With a response rate of 72%, this attribute indicates that the host is somewhat responsive but still does not meet higher standards of guest communication. While better than a 61% rate, it is still relatively low. This may still lead to uncertainty for potential guests, thus adversely affecting the price.

    - host_neighbourhoodEmbajadores (Estimate: -210.28)
      - Interpretation: The Embajadores neighborhood shows the most significant negative influence on price. Such a drastic estimate could mean Embajadores is viewed very negatively compared to other areas, possibly due to factors like high noise levels, safety concerns, or being less appealing in terms of local attractions and amenities.
