# Tips for PyTorch

### optimizer.zero_grad()
The gradients calculated in the last epoch/step will be saved in the optimizer buffer. In most cases, we want the optimizer to update the model parameters based on the batch gradients, then we need to clean the buffer at each epoch/step. However, sometimes we might need gradients from previous epochs/steps. For example:
+ When we want a huge batch size but only have a small GPU memory.
+ When we want to do a special moving average (or filtering) on the gradients.
+ etc.
