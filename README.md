

# Origin And Services
- **ISKCON Overview**

In 1965, Prabhupada embarked on a journey to the United States with the vision of initiating a global Hare Krishna movement. The inception of ISKCON took place in NYC in 1966 under Prabhupada's guidance. Over the next 11 years, he successfully established more than 100 centers, temples, and diverse projects.

The expansion of ISKCON extended to Bangalore in 1987, culminating in the construction of a significant temple in 1997. Presently, ISKCON boasts a network of over 100 temples worldwide.

ISKCON Bangalore is dedicated to social work and well-being, actively engaging in various initiatives. Their activities encompass pilgrimages, cow protection, food distribution, and spiritual programs, reflecting their commitment to holistic community service.

- **Challenges Faced**

The online presence team of ISKCON gathered feedback from social media to enhance services. However, they encountered challenges in manually handling the feedback. ISKCON was in need of an automated solution for analyzing sentiments, identifying trends, emotions, and addressing top issues derived from visitor feedback. The reviews collected exhibited issues such as multiple languages, spelling errors, and duplication. Analyzing mixed and neutral classes in the reviews posed challenges during the analysis process.

# Problem Statement

The problem statement primarily handles 4 points:

 1. Feedback Collection: The ISKCON online presence team actively gathers visitor feedback from social media platforms to enhance their services.

 2. Manual Effort Challenges: Despite the commitment to improving services, the team faced challenges in manually handling the collected feedback.

 3. Automated Solution Need: Recognizing the limitations of manual efforts, ISKCON sought an automated solution to perform sentiment analysis, identify trends, emotions, and address top issues derived from visitor feedback.

 4. Review Challenges: The collected reviews presented challenges such as multiple languages, spelling errors, and duplication. Additionally, the classification of mixed and neutral classes in the reviews posed difficulties during the analysis process.

# Data Overiew:

The data was given for a period of 5 years:
- 5685 reviews
-  Reveiws from Jan 2013 to Aug 2017


![image](https://github.com/Vishweshpurohit/Enhancing-Visitor-experience-at-ISKCON-using-text-analytics/assets/111001693/fe8cd9ed-d83a-42d6-b50b-7baa9f445419)

- 4 review sources
  
![image](https://github.com/Vishweshpurohit/Enhancing-Visitor-experience-at-ISKCON-using-text-analytics/assets/111001693/63ead463-5df3-4a08-a808-bd323178b4c4)

- 6 categories of rating
  
![image](https://github.com/Vishweshpurohit/Enhancing-Visitor-experience-at-ISKCON-using-text-analytics/assets/111001693/4a6a6585-43a3-4245-94db-e3e5d07727f3)

With four review sources, TripAdvisor has the most reviews, highlighting its importance for gathering visitor feedback. There are various review types, with a higher number of positive feedbacks and fewer queries and suggestions.

# Data Issues

## Handling Data Issues

| Issue                   | Remedy                                                             |
|-------------------------|--------------------------------------------------------------------|
| Duplicate Review        | Combine columns 'Source', 'Review By', and 'Review Date'. Filter duplicates based on this combined column. |
| Data Inconsistencies    | Address inconsistencies between review subject and review text columns by [your remedy here]. |
| Review text in languages other than English   | Performed language detection to identify and remove non-English text. |



## Exploratory Data Analysis

The number of reviews collected has significantly increased in recent times, with the highest volume of reviews gathered during the second quarter of 2017

![image](https://github.com/Vishweshpurohit/Enhancing-Visitor-experience-at-ISKCON-using-text-analytics/assets/111001693/be5b36b2-c67e-42ac-aad1-057d800ab799)

The first quarter of each year has consistently exhibited lower average ratings compared to the second and third quarters

![image](https://github.com/Vishweshpurohit/Enhancing-Visitor-experience-at-ISKCON-using-text-analytics/assets/111001693/b55c0043-e3e1-428d-ab5a-eb83dd9eb5a6)

According to the manual labels, positive reviews consistently outnumber negative and mixed reviews each quarter. The limited number of neutral reviews may suggest that people tend to express sentiment rather than merely stating facts in their reviews

![image](https://github.com/Vishweshpurohit/Enhancing-Visitor-experience-at-ISKCON-using-text-analytics/assets/111001693/9cd8ff90-cdfd-44c3-ba8c-6b83f95c5c0e)

## Sentiment Analysis

![image](https://github.com/Vishweshpurohit/Enhancing-Visitor-experience-at-ISKCON-using-text-analytics/assets/111001693/7ab0451e-f257-46b7-a6dc-4497c7ecbecc)


The prevalence of positive sentiment in reviews, ranging from 80 to 95%, indicates that individuals are more inclined to share favorable experiences about devotional places rather than offering criticism

![image](https://github.com/Vishweshpurohit/Enhancing-Visitor-experience-at-ISKCON-using-text-analytics/assets/111001693/3dca2b4b-e712-4514-927c-f088e94e8663)

Over time, there has been a noticeable decrease in the negative sentiment expressed in reviews. This trend suggests that efforts to address concerns and improve the overall experience at the ISKCON have been successful, leading to a more satisfying experience for visitors

![image](https://github.com/Vishweshpurohit/Enhancing-Visitor-experience-at-ISKCON-using-text-analytics/assets/111001693/45b95020-e2df-498b-a8c4-2908db4c8a64)

## Emotional Analysis

The majority of reviews showcase emotions such as positivity, joy, trust, and anticipation, indicating that ISKCON is providing visitors with a positive and uplifting experience. A minimal number of reviews express emotions like anger, sadness, or disgust, further emphasizing the overall satisfaction and enjoyment experienced by guests at the devotional place. This highlights ISKCON's success in creating a welcoming and spiritually enriching atmosphere for its visitors

![image](https://github.com/Vishweshpurohit/Enhancing-Visitor-experience-at-ISKCON-using-text-analytics/assets/111001693/4fc540ab-1521-4d50-b778-19a8c9754271)



## Short Term Recommendations

| Recommendation                                        | Implementation Steps                                       |
|-------------------------------------------------------|-------------------------------------------------------------|
| Make description mandatory to avoid empty descriptions | Add validation checks to make description fields mandatory.  |
| Address subjectivity in ratings for clearer user sentiment | Implement clearer rating guidelines or tooltips for users.  |
| Note discrepancies between positive descriptions and low ratings | Set up automated alerts for significant inconsistencies.    |
| Implement a Likert scale with clear labels as an alternative to a 1-5 scale | Adjust the user interface to incorporate a Likert scale.     |

## Long Term Recommendations

| Recommendation                                        | Implementation Steps                                       |
|-------------------------------------------------------|-------------------------------------------------------------|
| Provide web form in regional languages to reduce user friction | Develop a multilingual web form to cater to regional users. |
| Use Google Translate for backend English output | Integrate Google Translate API for backend language support. |
| Standardize data collection with a web form (e.g., Google Forms) | Create and implement a standardized data collection web form. |
| Connect form to a database and visualization tool for quick analysis | Establish a connection between the web form, database, and visualization tool. |

## Conclusion

# Problem and Solution

| Problem | Solution Required |
|---------|-------------------|
| How can ISKCON reduce the manual effort and automate the current process? How can ISKCON create a user interface (UI) that will make the entire data analysis more efficient? | To enhance the process of gathering and analyzing visitor feedback, a simple web form can be created using Google Forms. This intuitive platform allows for seamless collection of reviews from visitors. As feedback is submitted, it can be directly stored in a Google Sheet or another suitable database. To further analyze and process the data, Python can be utilized to perform sentiment analysis, uncover trends, and extract valuable insights from the collected reviews. Lastly, the processed data can be visualized using Tableau or a similar data visualization tool, resulting in an engaging and interactive user interface. |
|How can ISKCON reduce the manual effort and automate the current process and How can ISKCON create a user interface (UI) that will make the entire data analysis more efficient | To make the review submission process more accessible and user-friendly, it's essential to ensure that the web form is available in various regional languages. This approach can significantly reduce the language barrier that many users may face, thereby encouraging a higher percentage of visitors to share their experiences.  To streamline the data analysis process, the backend can be integrated with Google Translate, automatically translating the collected reviews into English. |






