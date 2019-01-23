---
  layout:     post
  title:      Multitask learning in context of NLU
  date:       2019-01-01 
  summary:    NLU for skill based smart voice agents 
  categories: 
  cover-image: /images/post_9/thumbnail.png
  highlighted: true
---
## What is Multi Task Learning ?
While doing Machine Learning (ML), we generally care about enhancing for a specific measurement, regardless of whether this is a score on a specific benchmark or a business KPI. So as to do this, we by and large train a solitary model or a gathering of models to play out our ideal assignment. We at that point calibrate and change these models until their execution never again increments. While we can by and large accomplish satisfactory execution along these lines, by being laser-centered around our single errand, we disregard data that may enable us to improve on the metric we care about. In particular, this data originates from the preparation signs of related undertakings. By sharing portrayals between related assignments, we can empower our model to sum up better on our unique undertaking. This methodology is called Multi-Task Learning (MTL) and will be the subject of this blog entry. As machine learning is not restrictive to any single domain, so does the MTL, it is applicable in computer vision, natural language processing, speech recognition.

> "MTL improves generalization by leveraging the domain-specific information contained in the training signals of related tasks".  
-- ![Rich Caruana](https://doi.org/10.1016/j.csl.2009.08.003)

### Philosopy
1. **Way the human learns**: We often learn those tasks first, that provide us with the necessary skills to master more complex tasks. Eg. we first learn to read and write then the grammar.
2. **MTL as Inductive Transfer**: Inductive transfer can help model to improve by introducing an inductive bias and rather than just develop the hypothesis with only one task which will be very much focused to that, learn from other auxillary tasks also.
3. **Implicit Data Augmentation**: As various tasks have diverse type of noise, so the model that learns multiple tasks simultaneously is able to generalize better. Therefore, learning just T1 bears the danger of overfitting to errand T1, while learning T1 and T2 together empowers the model to get a better representation of features, because of the noise introduced by those tasks.
4. **Regularization**: As it helps in generalizing the learner by introducing the inductive bias, thats why we can consider it as a regularizer also. 
5. **Feature borrowing and attention focusing**: On the off chance that an undertaking is extremely loud or information is restricted and high-dimensional, it tends to be troublesome for a model to separate among significant and unessential highlights. MTL can help the model concentrate on those highlights that really matter as different tasks will give extra proof to the importance or immateriality of those highlights. A few highlights F1 are anything but difficult to learn for some task T1, while being hard to learn for another undertaking T2. This may either be on the grounds that T2 cooperates with the highlights in an increasingly intricate manner or in light of the fact that different highlights are obstructing the model's capacity to learn F1. Through MTL, we can enable the model to listen stealthily, for example, learn F1 through task T1.

### MTL in Deep Learning
1. Soft Parameter Sharing
2. Hard Parameter Sharing

### Deep Learning Researches
1. Deep Relationship Networks
2. Fully-Adaptive Feature Sharing
3. Cross-stitch Networks
4. Low supervision
5. A Joint Many-Task Model
6. Weighting losses with uncertainty
7. Tensor factorisation for MTL
8. Sluice Networks