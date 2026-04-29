# Automatic Pore Characterization in SEM Images of Foams Using a Fine-Tuned Segment Anything Model
_Authors: Yung-Chen Cheng, Zong-Yun Tsai, Chen-Yu  Bair, Shu-Kai Yeh, Chuin-Shan Chen_

Identifying and analyzing pores in scanning electron microscopy (SEM) images of foams is a labor-intensive task, often requiring manual annotation that limits reproducibility and throughput. This study proposes an automated framework for pore characterization based on a fine-tuned Segment Anything Model (SAM). Low-rank adaptation (LoRA) and targeted data augmentation—including geometric transformations, color jittering, Gaussian blurring, and synthetic scratch generation—are employed to adapt SAM to the domain of foam microstructures. The resulting ViT-H2 model achieves high precision (0.90) and recall (0.90) across both monodisperse and polydisperse foams, while reducing errors in pore anisotropy ratio and angle to $1.93\%$ and $5.83^{\circ}$, respectively. The predicted pore masks closely align with expert annotations, capturing both pore size distributions and anisotropy characteristics with high fidelity. Notably, the method enables high-throughput pore analysis that integrates seamlessly into materials characterization workflows. These results demonstrate the effectiveness of fine-tuned foundation models for automated microstructure analysis, offering a scalable, data-driven approach for the design and discovery of advanced foams and other porous materials.

### Data

The training dataset contains 64 SEM images and their corresponding manually labeled masks, stored in the `Training_Data` folder.

The evaluation dataset contains 6 challenging SEM images and their corresponding masks, stored in the `Evaluating_Data` folder. This dataset is used to assess the model's performance on complex SEM images.

### Citation
Cheng, Y. C., Tsai, Z. Y., Bair, C. Y., Yeh, S. K., & Chen, C. S. (2026). Automatic pore characterization in SEM images of foams using a fine-tuned segment anything model. Materials & Design, 262, 115529.