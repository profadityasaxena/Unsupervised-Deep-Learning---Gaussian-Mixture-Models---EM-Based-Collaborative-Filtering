
# 📊 Unsupervised Deep Learning: Gaussian Mixture Models & EM-Based Collaborative Filtering

Welcome to the official course repository for **"Unsupervised Deep Learning: Gaussian Mixture Models & EM-Based Collaborative Filtering"**, led by **Aditya Saxena**. This course is a deep dive into the foundational and advanced techniques of unsupervised learning, focusing on probabilistic models, clustering, and recommender systems.

This project-based course takes you through a journey beginning with the basics of unsupervised learning and gradually evolves into the application of **Gaussian Mixture Models (GMM)** and **Expectation-Maximization (EM)** for **matrix completion**. The final stages of the course apply these techniques to real-world data, such as the Netflix ratings dataset, and evaluate the performance using quantitative metrics like log-likelihood and RMSE.

## 📓 Course Modules
Each module consists of structured Jupyter Notebooks with explanations, derivations, code walkthroughs, and mini-projects.

1. **Module 01: Introduction to Unsupervised Learning**
2. **Module 02: K-Means Clustering**
3. **Module 03: Gaussian Mixture Models (GMMs)**
4. **Module 04: Expectation-Maximization (EM) Algorithm**
5. **Module 05: EM for Matrix Completion (Netflix Data)**
6. **Module 06: Log-Domain Calculations & Stability**
7. **Module 07: BIC for Model Selection**
8. **Module 08: Completing Missing Entries**
9. **Module 09: Evaluation using RMSE & Model Interpretability**
10. **Module 10: Final Project & Case Study Walkthrough**

## 🔍 Key Features
- Matrix Completion on Netflix Dataset using EM
- Derivations and Log-Likelihood Maximization
- Posterior and Prior probability calculations
- Numerical Stability with LogSumExp
- Model Selection using BIC
- Root Mean Squared Error Evaluation

## ❓ 50 Theory Questions and Answers

1. **What is unsupervised learning?**  
   Learning patterns from unlabeled data.

2. **Give an example of an unsupervised task.**  
   Clustering users based on movie preferences.

3. **What is the K-means algorithm?**  
   A clustering algorithm that partitions data into K clusters minimizing intra-cluster variance.

4. **What does the "K" in K-means refer to?**  
   The number of clusters.

5. **What is the limitation of K-means?**  
   It assumes equal spherical variance and hard assignment.

6. **What is a Gaussian Mixture Model?**  
   A probabilistic model that assumes all data points are generated from a mixture of several Gaussian distributions.

7. **What is the EM algorithm?**  
   An iterative optimization algorithm to estimate parameters in probabilistic models with latent variables.

8. **What are the two steps in EM?**  
   Expectation (E-step) and Maximization (M-step).

9. **What does the E-step compute?**  
   Posterior probabilities (responsibilities).

10. **What does the M-step compute?**  
    Parameters that maximize expected log-likelihood.

11. **What is a latent variable?**  
    A variable that is not directly observed but inferred from the model.

12. **What are responsibilities in EM?**  
    Probability that a data point belongs to a specific component.

13. **Why use log-likelihood?**  
    To avoid numerical underflow and for better optimization.

14. **What is logsumexp?**  
    A stable way to compute the log of sums of exponentials.

15. **Why is EM used for matrix completion?**  
    It can handle missing values naturally by marginalizing over unobserved dimensions.

16. **What is the marginal likelihood in matrix completion?**  
    The likelihood over only the observed dimensions.

17. **How are missing entries filled?**  
    Using the weighted average of Gaussian means based on responsibilities.

18. **What is the BIC criterion?**  
    Bayesian Information Criterion, used for model selection penalizing complexity.

19. **How is BIC computed?**  
    \[ \text{BIC} = \log L - \frac{p}{2} \log n \]

20. **What does 'p' stand for in BIC?**  
    Number of free parameters.

21. **What is RMSE?**  
    Root Mean Squared Error, a measure of prediction accuracy.

22. **Why evaluate with RMSE?**  
    It gives insight into prediction error magnitudes.

23. **Why use Gaussian mixtures over K-means?**  
    It allows soft assignments and models elliptical clusters.

24. **What is a soft assignment?**  
    A probability of belonging to a cluster instead of hard 0/1.

25. **What is spherical covariance?**  
    Variance is the same in all directions.

26. **Why use log domain in computation?**  
    For numerical stability when dealing with small probabilities.

27. **How are priors used in EM?**  
    As initial probabilities for each component.

28. **Why normalize responsibilities in E-step?**  
    To ensure they form a valid probability distribution.

29. **What happens if variance becomes too small?**  
    Numerical instability or overfitting.

30. **What is the minimum variance trick?**  
    To clip variance to a lower threshold to maintain stability.

31. **What is the stopping criterion in EM?**  
    Change in log-likelihood is less than epsilon times new log-likelihood.

32. **What is a mixture coefficient?**  
    The prior probability of a Gaussian component.

33. **What dataset is used in this project?**  
    Toy dataset and Netflix ratings.

34. **What does collaborative filtering mean?**  
    Predicting a user's interests using preferences of similar users.

35. **Why is matrix completion hard?**  
    Because of missing data and potential for overfitting.

36. **What are mini-projects in this course?**  
    Case studies solving real-world clustering and recommendation problems.

37. **Why do we use initialization seeds?**  
    To avoid poor local minima in EM.

38. **How is matrix completion different from matrix factorization?**  
    EM models data probabilistically; factorization optimizes latent features.

39. **What is the dimensionality of a data point in matrix completion?**  
    The number of items (movies) rated.

40. **What is the role of masks in matrix completion?**  
    To isolate observed vs. missing entries.

41. **What is the identity matrix in GMMs?**  
    Represents isotropic variance in Gaussian components.

42. **How are EM and GMM connected?**  
    EM is the algorithm used to estimate parameters in GMMs.

43. **Why plot clusters?**  
    To visually understand model behavior.

44. **What are convergence issues in EM?**  
    Getting stuck in local optima.

45. **How to address local optima?**  
    Use multiple seeds and select best log-likelihood.

46. **What does log-likelihood tell us?**  
    How well the model fits the data.

47. **How are Gaussian parameters updated?**  
    Using weighted means and variances.

48. **What is overfitting in EM?**  
    Too many clusters or small variance leading to memorization.

49. **How is overfitting avoided in GMM?**  
    Through BIC and minimum variance constraints.

50. **Why is this project important?**  
    It demonstrates real-world application of probabilistic modeling to recommender systems.

---

Stay tuned for more notebooks, challenges, and mini-projects!

> Instructor: Aditya Saxena  
> GitHub: [@profadityasaxena](https://github.com/profadityasaxena)

---
