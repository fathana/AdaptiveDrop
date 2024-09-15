# AdaptiveDrop

This repository is for our paper currently under review. The code of our experiments will be available upon acceptance of our paper. We also include below additional ablation studies for our proposed AdaptiveDrop filtering framework.

# AdaptiveDrop: metrics over epochs
In Figure 3, we show the evolution of several metrics over epochs using AdaptiveDrop versus only using the loss functions. Here we use CAMSAT-based pseudo-labels.
![](/AdaptiveDrop_metrics_over_epochs.png)

# AdaptiveDrop: the case of other pseudo-labels
In Table 5, we show a comparison study of our four main losses used to train our SV models with and without AdaptiveDrop across various pseudo-labels. Results show clearly that our AdaptiveDrop boosts SV performance across all the pseudo-labels studied.
![](/AdaptiveDrop_versus_without_all_pseudo_labels.png)

# Noisy labels correction
Table 6 shows the final label unsupervised clustering accuracy across all our different pseudo-labels. Using unsupervised clustering accuracy (ACC) to measure the consistency between the ground-truth labels
and the initial clustering-driven PLs or the final rectified PLs. We can observe that improvements thanks to our label correction module vary depending on the type of PLs used to train the network, and that AdaptiveDrop helps to enhance label accuracy across all the pseudo-labels. For instance, we got up to 9% improvement in ACC after training completed in case of the GMM-based PLs. This is equivalent to more than 98,280 successfuly corrected noisy samples in the VoxCeleb2 dataset, which shows that label correction can be tremendously beneficial to boost SV performance and speaker clustering. ![](/Label_accuracy_all_pseudo_labels.png)

# AdaptiveDrop: Evaluation on other datasets.
Table 8 shows the evaluation of our SV model trained using different losses with/without AdaptiveDrop. For evaluation, we use the 3 Voxceleb1 evaluation sets: Vox1-O, Vox1-E, and Vox1-H. ![](/AdaptiveDrop_evaluation_other_datasets.png)
