# fantasy_name_generator
Machine learned fantasy name generator,
based on this [pokemon-name-generator](https://github.com/simon-larsson/pokemon-name-generator/blob/master/name_generator.ipynb) by simon-larsson.

## Install
This project uses `poetry` to install and maintain python libraries.
```
$ poetry install
```

## Use
### Setup
```
1) Put a <filename>.txt in the data folder
	* There should be exactly one name on each line.
2) Edit the settings in src/ml/settings.py
```

### Training and Generating
Run the training, it will also generate 10 names (by default).
```
$ poetry run generate -s <filename>.txt
```

If you already have a model trained, you can use the `-l` flag. This will load the model from the path speciefied in `src/ml/settings.py` and generate an amount of names specified.
```
$ poetrun run generate -s <filename>.txt -l
```
