# generalizing_IFs
The notebooks in this repo are implementations of a series of examples from https://arxiv.org/abs/1411.4342 and https://arxiv.org/abs/2107.00681


The main notebooks for demonstrating IFs for bias reduction are:

- ATE-NN-separate_model_training_TREG.ipynb -> this has seperate Q and G NNs, applies targeted regularization to the Q network, and provides a comparison of the performance for the network with the same hyperparameters without targeted reg.
- ATE-NN-separate_model_training_ONESTEP_AND_SUBMODEL.ipynb -> this has separate Q and G NNs and compares the one-step update, the submodel/regression update, and the naive model (no IFs).
- ATE.ipynb -> this follows a similar process to https://github.com/migariane/SIM-TMLE-tutorial and shows the various scenarios (one-step, submodel, misspecified Q, misspecified G etc.) and corresponding bias reduction (if any).
- k-fold_conditional_expectation.ipynb -> Provides a demonstration of bias reduction (or not) depending on the misspecification of the outcome model.
- generalising_IFs_autograd_tutorial-SIMS.ipynb  -> demonstrates bias reduction for estimation of Shannon entropy using autograd for the functions (can be generalised slightly beyond entropy to arbitrary functions phi() and nu()). Follows https://arxiv.org/abs/1411.4342



