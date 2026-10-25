# Model Optimization

Hands-on exercises for learning the core ideas of **model optimization** for edge deployment.

## The five ideas

| # | Exercise | One line | Core to focus on |
|---|----------|----------|------------------|
| 1 | [Quantization](examples/01_quantization.ipynb) | Use fewer bits to represent numbers | quantization scheme & formula, compression ratio |
| 2 | [Knowledge Distillation](examples/02_knowledge_distillation.ipynb) | A big model teaches a small one | distillation loss formula, teacher-student architecture |
| 3 | [Pruning](examples/03_pruning.ipynb) | Remove unused signals | granularity, ratio, criteria |
| 4 | [Neural Architecture Search](examples/04_nas.ipynb) | Search for an optimal architecture | search space & strategy |
| 5 | [Kernel Optimization](examples/05_kernel_optimization.ipynb) | Make the same math run faster on the GPU | tiling, grid layout, memory access |


Kernel optimization is more hardware-constrained and usually speeds up the computation without changing the math.
Meanwhile, the remaining ideas are more abstract and usually change what the model computes.
They are orthogonal in concept and may be coupled in realization. For example, a **quantized matmul kernel** is entirely possible.

## How to run

### Google Colab

1. Open the notebook for an exercise (links above).
2. Click **"Open in Colab"** (badge at the top of each notebook), or upload the `.ipynb`
   to Colab manually.
3. Set the runtime to **GPU** (`Runtime -> Change runtime type -> GPU`).
4. `Runtime -> Run all`.

