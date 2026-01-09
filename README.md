BLUF: 

* Large Language Models share a universal pattern in the magnitude of their transformer block activations which replicates accross model familes, and parameter counts.
* This universal invariant emerges fairly early in training, and is extremely stable.
* This structure can serve as an internal diagnostic lens for training dynamics and potential failure modes.


**Abstract**

Large Language Models (LLMs) not only differ in performance, but also in how they distribute
computation across depth. In this work, we identify a remarkably consistent three-phase activation
pattern that emerges during training and recurs across diverse decoder-only transformers. Analyzing
layer-wise ℓ1-activations on paired abstract and literal prompts for 60 models, we find that sufficiently
large architectures exhibit a conserved depth profile characterized by an early-layer extremum, a
suppressed mid-layer plateau, and a late-layer surge—a structural motif we term the Hau Curve. This
pattern appears as the dominant mode of variation in a principal component analysis (PC1 accounting
for roughly one-third of variance in dense-condition activations). Developmental analyses show
that it arises early in pretraining (≈ 7,000 steps for a 12B model) and then stabilizes, suggesting
a training-induced attractor in network dynamics. Notably, the effect is weak or inconsistent in
architectures with fewer than ∼20–24 transformer blocks, and stabilizes in models with ≥30–32 blocks,
indicating a depth-dependent emergence threshold rather than a purely parametric one. Together, these
findings position the Hau Curve—and its convergence behavior, the Hau Attractor—as fundamental
structural properties of transformer LLMs, revealing intrinsic architectural dynamics not observable
from model behavior alone.

