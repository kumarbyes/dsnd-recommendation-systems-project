# Recommendation System Project: IBM Community

![RecommendationSystems](starter/images/recommendation_systems.png)

## Table of Contents

- [Project Description](#project-description)
- [Dataset](#dataset)
- [Requirements](#Requirements)
- [Installations](#Installations)
- [File description](#file-description)
- [Result summary](#Result-summary)
- [License](#license)

## Project Description

This project recommends articles to the users in IBM Watson studio. The workflow is sectioned into different recommendation systems. Starting with rank-based recommendation systems where the top articles with highest interactions are suggested to the user. Then user-user collaborative filtering was used to recommend articles where the users are grouped based on similarity to other users. This way the article read by an user can be suggested to other users who are similar. Moving on content based recommendation system was implemented to group similar articles using kMeans clustering techniques. In this recommendation engine, user-user interactions are not required. An user is suggested new articles based on the articles he/she has read. Articles belonging to the same clusters are suggested to the user. Finally, Matrix factorization (SVD) was used to recommend articles based on article similarity. Each recommendation engine serves a purpose.

### Dataset

There are 3 features in the dataset for recommending articles to the user in IBM Watson Studio.

The features can be summarized as the following:

- **article_id**: Integer variable that refers to the id of the article
- **title**: text variable that refers to the title of the article
- **email**: encrypted email id of the user

### Requirements

-**Python Version**: 3.11.9 was used for this project<br/>
-Jupyter notebook was used for the complete development of this project<br/>
-Check Requirements.txt file for all the libraries used in the project<br/>

### Installation

Install the required libraries for the project using **requirements.txt** file:

```bash
pip install -r requirements.txt
```

### File description

Following files are available in the github repository to succesfully run the code:

1. **Recommendations_with_IBM.ipynb**: This is primary file containing all the relevant python code for project. At each point in the notebook, markdown cells are added to explain the process or inform about the inference.
2. **Requirements.txt**: Python libraries used in the project for pip install
3. **user-item-interactions.csv**: Csv file containing the data needed for the recommendation systems
4. **LICENSE.txt**: License file for the project

### Result Summary

**Ranking-based**: Used when there is no user history available or for new users.
**User-User collaborative filtering**: Used when enough user-item interactions are present
**Content based systems**: used when there is less user-user relationship. has better scope to integrate machine learning models
**Matrix factorization (SVD)**: used when user-item matrix is sparse. finds latent features which are not observed but inferred

Each recommendation engines has its own pros and cons. It is always better to use a comination of recommendation engines based on the needs.

## License

[License](LICENSE.txt)
