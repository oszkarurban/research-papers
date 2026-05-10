# Research Papers

A collection of papers and project reports I have authored or co-authored at the
University of Cambridge and ETH Zurich. Topics span LLM interpretability and
activation steering, vision-language model robustness, multimodal medical AI,
and computational linguistics for low-resource languages.

## Papers

### [University of Cambridge — Improving MCQ Performance via Activation Steering of Query Styles](Cambridge_activation_steering_for_mcq.pdf)
Extracts persona vectors (polite, insulting, urgent, …) from internal LLM
activations and steers along them at inference time, improving accuracy on
MMLU Math, TruthfulQA, RACE and Mind Your Tone by up to 12.5% while reducing
prediction entropy and Expected Calibration Error.
*Code: [oszkarurban/l101-activationsteering](https://github.com/oszkarurban/l101-activationsteering)*

### [ETH Zurich — Adversarial Testing of WebAgents (SRILab)](ETH_Zurich_adversarial_testing_webagents.pdf)
Implements PGD-based adversarial image attacks against VisualWebArena VLM
agents (BLIP-2 / FLAN-T5), increasing the length of enforceable adversarial
captions from 4 to 19 tokens via Adam optimisation and a custom
gradient-friendly image preprocessor.
*Code: [oszkarurban/pgd](https://github.com/oszkarurban/pgd)*

### Samsung AI — Adaptive Speculative Decoding for Chain-of-Thought Reasoning Models
Replace the static draft-tree configuration used by current
speculative decoders with an adaptive controller that reads internal signals
from the residual stream — token-level entropy, hidden-layer activation
patterns, and reasoning-dynamics features across the CoT trace — and uses them
to gate speculative-tree expansion at inference time, relaxing during
exploratory thinking phases and tightening during high-stakes answer phases.
Achieves ~30% throughput improvement over SoTA EAGLE-3.
*Code available on request.*

### [University of Cambridge — Multimodal Framework for Alzheimer's Disease Classification and Stable Attribution](Cambridge_alzheimers_multimodal.pdf)
Joint work fusing 3D T1-weighted MRI with structured clinical text (3D ViT +
ModernBERT, late fusion) and using Sparse Autoencoders together with UMAP
geometric constraints to recover stable, clinically consistent feature
attributions across in-distribution and out-of-distribution cohorts.

### [University of Cambridge — Hungarian Minimal Pairs for Negation-Induced Preverb Inversion](Cambridge_hungarian_minimal_pairs.pdf)
Introduces a Hungarian minimal-pair benchmark targeting preverb inversion
under negation, evaluates monolingual and multilingual LMs across four
lexical-complexity levels, and uses mechanistic analysis to attribute failures
to tokenisation artifacts and attention collapse.
*Code: [oszkarurban/l95-minimalpair](https://github.com/oszkarurban/l95-minimalpair)*

### [University of Cambridge — Assessing the Transferability of Text LLMs for Protein Inverse Folding via Structural Tokenization](Cambridge_LLM_proteininversefolding_GNN.pdf)
Discretises 3D protein backbones into 1D token strings (Foldseek's 3Di alphabet
and C-α coordinate strings) and probes whether linguistic priors from a
pretrained Llama-3-8B transfer to inverse protein folding; LoRA fine-tuning
recovers meaningful sequence-recovery gains over a randomly initialised
baseline, showing that text-LLM inductive biases provide a usable foundation
for protein design without architectural changes.
