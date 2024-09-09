# AdaptiveDrop

This repository is for our paper entitled "ADAPTIVEDROP: A SIMPLE ADAPTIVE LABEL NOISE FILTERING SCHEME
FOR ENHANCED SELF-SUPERVISED SPEAKER VERIFICATION" currently under review.

Code of our experiments will be available upon acceptance of our paper. We also include below additional ablation studies for our proposed AdaptiveDrop filtering framework.

# AdaptiveDrop: metrics over epochs
In Figure 3, we show the evolution of several metrics over epochs using AdaptiveDrop versus only using the loss functions. Here we use CAMSAT-based pseudo-labels.
![](/AdaptiveDrop_metrics_over_epochs.png)

# AdaptiveDrop: the case of other pseudo-labels
In Table 5, we show a comparison study of our four main losses used to train our SV models with and without AdaptiveDrop across various pseudo-labels. Results show clearly that our AdaptiveDrop boosts SV performance across all the pseudo-labels studied.
![](/AdaptiveDrop_versus_without_all_pseudo_labels.png)

# Noisy labels correction
Table 6 shows the final label unsupervised clustering accuracy across all our different pseudo-labels. results show that AdaptiveDrop helps to enhance the label accuracy across all the pseudo-labels used: ![](/Label_accuracy_all_pseudo_labels.png)

# AdaptiveDrop: Evaluation on other datasets.
Table 8 shows the evaluation of our SV model trained using different losses with/without AdaptiveDrop. For evaluation, we use the 3 Voxceleb1 evaluation sets: Vox1-O, Vox1-E, and Vox1-H. ![](/AdaptiveDrop_evaluation_other_datasets.png)
