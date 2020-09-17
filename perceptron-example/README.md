## Ejemplo perceptron

### Definimos dos arreglos conn los valores reales de entrada y salida de unna compuerta logica, en este caso es una compuerta OR.

```py
X = np.array([[0, 0],[0, 1],[1, 0],[1, 1]])
y = np.array([[0],[1],[1],[1]])
```

# Iniciamos el entrenamiento de nuestro perceptron solo usando los datos de entreda. Como dato adicional definimos que sera entrenando durante 20 ciclos con un porcentaje de aprendizaje igual a 0.1.

```py
p = Perceptron(X.shape[1], alpha=0.1)
p.fit(X, y, apochs=20)
```

### Ejecutamos main.py

```ssh
python main.py
```

resultado

```ssh
Resultado: entradas=[0 0], valor real=0, valor predicho=0
Resultado: entradas=[0 1], valor real=1, valor predicho=1
Resultado: entradas=[1 0], valor real=1, valor predicho=1
Resultado: entradas=[1 1], valor real=1, valor predicho=1
```
