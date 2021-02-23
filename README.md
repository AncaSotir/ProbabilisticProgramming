# Probabilistic Programming

This repo contains two projects on Probabilistic Programming. The notebooks in html format can also be found in this repo.

1. **Latent Dirichlet Allocation (LDA) in PyMC**

    Given a set of documents from different topics, the main goal is:
      - to infer the documents distribution over the topics
      - to infer the topic distribution over the vocabulary

    [image for visualizing topics]
    [image for visualizing document]
  
    Additional tasks:
      - topic-based similarity between documents
      - assign topic to a new document

    [image for similarity matrix]
    [image for visualizing topic assigned to a new document]


2. **Bayesian Learning for Neural Networks in Pyro**

    The task: comparing bayesian networks and classic neural networks.
    This comparison is done by considering the following tasks:
      - a linearly separable binary classification problem
      - a non-linearly separable binary classification problem
      - a multinomial classification problem
    Extra experiment: in the case of bayesian networks, the weights and bias are inferred; inference over the network architecture (i.e. hidden layer size) was also attempted.
    
    [images with the problems]
    
    Result summary:
      Problem type | Bayesian Network results | Classic Network results | Notes
      --- | --- | --- | ---
      Binary classification (linearly separable) | 100% test acc. | 100% test acc. | Sanity check, same results, simple and quick inference/training
      Binary classification (non-linearly separable) | 95% test acc. | 96% test acc. | More complex problem, same results, neccesity of more complex networks and more inference/training time
      Multinomial classification | 80% test acc. | 90% test acc. | The classic network clearly outperformed the bayesian network
