# Research Papers

A collection of papers and project reports I have authored or co-authored at the
University of Cambridge and ETH Zurich. Topics span LLM interpretability and
activation steering, vision-language model robustness, multimodal medical AI,
and computational linguistics for low-resource languages.

## Papers

### [L101 — Improving MCQ Performance via Activation Steering of Query Styles](L101_activation_steering_for_mcq.pdf)
Extracts persona vectors (polite, insulting, urgent, …) from internal LLM
activations and steers along them at inference time, improving accuracy on
MMLU Math, TruthfulQA, RACE and Mind Your Tone by up to 12.5% while reducing
prediction entropy and Expected Calibration Error.
*Code: [oszkarurban/l101-activationsteering](https://github.com/oszkarurban/l101-activationsteering)*

### [Adversarial Testing of WebAgents (ETH SRILab)](ETH_adversarial_testing_webagents.pdf)
Implements PGD-based adversarial image attacks against VisualWebArena VLM
agents (BLIP-2 / FLAN-T5), increasing the length of enforceable adversarial
captions from 4 to 19 tokens via Adam optimisation and a custom
gradient-friendly image preprocessor.
*Code: [oszkarurban/pgd](https://github.com/oszkarurban/pgd)*

### [L205 — Multimodal Framework for Alzheimer's Disease Classification and Stable Attribution](L205_alzheimers_multimodal.pdf)
Joint work fusing 3D T1-weighted MRI with structured clinical text (3D ViT +
ModernBERT, late fusion) and using Sparse Autoencoders together with UMAP
geometric constraints to recover stable, clinically consistent feature
attributions across in-distribution and out-of-distribution cohorts.

### [L95 — Hungarian Minimal Pairs for Negation-Induced Preverb Inversion](L95_hungarian_minimal_pairs.pdf)
Introduces a Hungarian minimal-pair benchmark targeting preverb inversion
under negation, evaluates monolingual and multilingual LMs across four
lexical-complexity levels, and uses mechanistic analysis to attribute failures
to tokenisation artifacts and attention collapse.
*Code: [oszkarurban/l95-minimalpair](https://github.com/oszkarurban/l95-minimalpair)*
