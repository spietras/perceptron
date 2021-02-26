# perceptron
Multilayer Perceptron Library 🧠

## Example usage

```python
from models import MultiLayerPerceptron

X_train, Y_train, X_test, Y_test = ...

mlp = MultiLayerPerceptron(X_train.shape[1], Y_train.shape[1], hidden_layers_sizes=[2*X_train.shape[1]])
history = mlp.fit(X_train, Y_train, epochs=100)
Y_pred = mlp.predict(X_test)
```

## Tests

You can also test it for iris classification. Run from cmd from top directory:

```sh
python test.py [-l LEARNING_RATE] [-k K_FOLD] [-e EPOCHS] [-b BATCH_SIZE] neurons ...
```
