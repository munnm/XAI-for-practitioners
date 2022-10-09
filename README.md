*This is not an official Google product*

# XAI-for-practitioners
Code for the O'Reilly book on Explainability methods for the ML practitioner.

### Title: Explainable AI for Practitioners

<img src="Explainable_AI_for_Practitioners.png" alt="XAI_for_practitioners" width="400"/>

## Table of Contents
0. Preface
1. Introduction
   - Why Explainable AI?
   - Who needs Explainability?
   - Challenges in Explainability
   - Evaluating Explainability
   - How Has Explainability Been Used

2. Overview of Explainability 
   - What are Explanations?
   - Explainability Consumers
     - Practitioners – Data Scientists & ML Engineers
     - Observers – Business Stakeholders & Regulators
     - End-Users – Domain Experts & Affected Users
   - Types of Explanations
     - Pre-modeling explainability
     - Intrinsic vs Post-Hoc Explainability
     - Local, Cohort and Global Explanations
     - Attributions, Counterfactual, and Example-based
   - Themes throughout Explainability
     - Feature Attributions
       - Shapley Values
       - Gradient-based Techniques
       - Saliency maps and feature attributions
    - Surrogate models
    - Activation

3. [Explainability methods for tabular data](./03-tabular)
   - [Permutation Feature Importance](./03-tabular/permutation_feature_importance.ipynb)
   - [Shapley Values](./03-tabular/SHAP.ipynb)
     - Visualizing local feature attributions
     - Visualizing global feature attributions
     - Interpreting Feature Attributions from Shapley Values
     - Managed Shapley values
   - [Explaining Tree Based Models](./03-tabular/treeinterpreters.ipynb)
     - From Decision Trees to Tree Ensembles
     - SHAP's TreeExplainer
   - Partial Dependence Plots & Its Relatives
     - [Partial Dependence Plots](./03-tabular/pdp_plots.ipynb)
       - Working with classification models
       - Assumption of independence
       - Understanding feature distributions
     - [Individual Conditional Expectation plots](./03-tabular/ice_plots.ipynb)
     - [Accumulated Local Effects](./03-tabular/ale_plots.ipynb)
     
4. [Explainability methods for image data](./04-image)
   - [Integrated Gradients](./04-image/integrated_gradients.ipynb)
     - Choosing a baseline
     - Accumulating Gradients
     - Improvements on Integrated Gradients
       - Blur Integrated Gradients
       - Guided Integrated Gradients
   - [XRAI](./04-image/xrai.ipynb)
     - How XRAI works
     - Implementing XRAI
   - [Grad-CAM](./04-image/grad-cam.ipynb)
     - How Grad-CAM works
     - Implementing Grad-CAM
     - Improving Grad-CAM
   - [LIME](./04-image/LIME.ipynb)
     - How LIME works
     - Implementing LIME
   - [Guided Backpropagation and Guided Grad-CAM](./04-image/guided_backprop_pytorch.ipynb)
     - Guided Backprop and DeConvNets
     - Guided Grad-CAM

5. [Explainability methods for text data](./05-text)
   - Overview of building models with text
     - Tokenization
     - Word embeddings and pre-trained embeddings
   - [LIME](./05-text/LIME_for_text.ipynb)
     - How LIME works with text
   - [Gradient x Input](./05-text)
     - Intuition from Linear Models
     - From Linear to Non-linear and Text Models
     - Grad L2-norm
       - Comparing sensitivity and saliency methods
   - [Layer Integrated Gradients](./05-text/layer_integrated_gradients.ipynb)
     - A Variation on Integrated Gradients
   - [Layer-wise Relevance Propagation (LRP)](./05-text/LRP_bert_explainability.ipynb)
     - How LRP works
       - The relationship between LRP and Grad x Input
     - Deriving explanations from Attention
   - Which method to use?
     - [Language Interpretability Tool](https://pair-code.github.io/lit/)

6. Advanced and emerging topics (with Sheeraz Ahmad)
   - Alternative Explainability Techniques
     - Alternate Input Attribution
       - Example-based Explanations
       - Influence Function-based Explanations
       - Concept-based Explanations
     - Explainability by Design
   - Other Modalities
      - Time-series Data
      - Multimodal Data
   - Evaluation of Explainability Techniques
     - A Theoretical Approach
     - Empirical Approaches

7. Interacting with Explainability
   - Who uses Explainability?
   - How to display Explanations
   - Clarity in explanations
   - Accuracy in explanations
   - Building on existing understanding
   - Common pitfalls in using Explainability

8. Putting it all together
   - Building with explainability in mind
     - The ML Life Cycle
       - Explainability through Discovery
       - Explainability through Development
       - Explainability through Deployment
   - AI regulations and explainability
   - What to look forward to in Explainable AI
     - Natural Explanations
     - Interrogative Explanations
     - Targeted Explanations

9. Appendix: Taxonomy, Techniques,& Further Reading
   - ML Consumers
   - Taxonomy of Explainability
   - XAI Techniques
     - Tabular Models
     - Image Models
     - Text Models
     - Advanced Techniques
   - Interacting with Explainability
   - Putting it all together
   - Further Reading
