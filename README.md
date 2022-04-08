# digits
L’un des projets les plus basiques dans le machine learning est l’analyse du dataset load_digits de sklearn, ce jeu de données est composé de plusieurs images de chiffres allant de 0 à 9 en 2D.

Un réseau de neurones sera utilisé pour détecter le chiffre qui est visualisé dans les différentes images avec la library Tensorflow.

Après avoir charger le jeu de donnée et créer 2 variable feature dont sa valeur est l’ensemble des images et targets dont sa valeur est l'étiquette de chacune des images, j’ai standardiser les images afin que le modèle puisse les comprendre correctement, puis divisé le feature et le target en données de test, et en données d'entraînement.

Après ceci j’ai entamé la phase de la modélisation, en utilisant un modèle séquentiel avec 256 layers d'entrée avec la fonction d’activation “relu”, 128 hidden layers avec également la fonction d’activation “relu” et 10 layers de sortie avec la fonction d’activation “softmax”, ensuite j’ai lancé une prédiction pour voir comment il effectue la prédiction pour avoir un résumé sur la prédiction du modèle.

Suite a ca j’ai utilisé la méthode compile pour optimiser les prédictions du modèle avec une fonction loss “sparce_categorical_crossentropy”, un optimiser “sgd” et une metric en accuracy et ensuite l'entraîner le modèle avec 50 “Epoch”.

Après l'entraînement j’ai essayé d’en savoir un peu plus en visualisant ce qui s’est passé pendant l'entraînement, le Loss d'entraînement et de la validation du Loss d'entraînement sont devenu faible a chaque nouveaux “Epoch” et l’accuracy de l'entraînement et de la validation était correcte, donc le modèle converge correctement.

Puis j’ai utilisé le modèle pour qu’il puisse identifier le nombre 7 sur une image et le modèle l'a identifié correctement.
