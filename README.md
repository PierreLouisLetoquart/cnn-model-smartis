# cnn-model-smartis

Ce répo contient le code Python pour entraîner et utiliser un modèle de réseau de neurones convolutif (CNN) afin de classer des images concernant des problèmes de voirie dans le cadre du projet Smart'is. L'application permet aux utilisateurs de prendre des photos avec leur téléphone portable de problèmes de voirie tels que des graffitis, des objets abandonnés ou des nids de poule, et d'envoyer ces photos à l'application. Le modèle de CNN est ensuite utilisé pour classer l'image reçue et comprendre à quelle classe de problème la photo appartient. L'application contactera ensuite automatiquement le bon service pour traiter le problème.

## Prérequis

- Python 3.10 ou plus
- Jupyter Notebook
- Les bibliothèques Python suivantes : tensorflow, keras, numpy, matplotlib, opencv-python, pillow

## Utilisation

- Clonez ce répo sur votre machine locale :

```sh
git clone git@github.com:PierreLouisLetoquart/cnn-model-smartis.git
```

- Créez un dossier `dataset` à la racine du répo et ajoutez-y les images d'entraînement selon l'arborescence suivante :

```markdown
dataset/
  train/
    class1/
      image1.jpg
      image2.jpg
      ...
    class2/
      image1.jpg
      image2.jpg
      ...
    ...
  validation/
    class1/
      image1.jpg
      image2.jpg
      ...
    class2/
      image1.jpg
      image2.jpg
      ...
    ...
```

- Utilisez le notebook `preprocessing.ipynb` pour prétraiter les images d'entraînement avant de les utiliser pour l'entraînement et la prédiction du modèle de CNN.
- Utilisez le notebook `model.ipynb` pour entraîner le modèle de CNN sur les images prétraitées et sauvegarder le modèle entraîné.
- Utilisez le notebook `prediction.ipynb` pour faire des prédictions sur de nouvelles images en utilisant le modèle entraîné.
