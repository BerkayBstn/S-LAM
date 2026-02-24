# S-LAM
Local Attention Mechanism for time series forecasting proposed by Martos et al. This repo fixes bugs in the script provided by the authors and improves efficiency by applying SDPA and parallelizing mask calculation. The current implementation also handles reconfiguring masks if a sequence with a different length is input to the model, whereas in the original application the configuration happens only once, and providing a different sequence length causes an error.

# Reference

@article{aguilera2024local,
  title={Local Attention Mechanism: Boosting the Transformer Architecture for Long-Sequence Time Series Forecasting},
  author={Aguilera-Martos, Ignacio and Herrera-Poyatos, Andr{\'e}s and Luengo, Juli{\'a}n and Herrera, Francisco},
  journal={arXiv preprint arXiv:2410.03805},
  year={2024}
}
