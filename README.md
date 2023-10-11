### Detection-des-fraudes-des-transactions-par-carte-de-credit-Radom-Forest-reseaux-de-neurones ###
Dataset (Train and test)
Source des données: https://www.kaggle.com/datasets/kartik2112/fraud-detection

### Encoding ###

Colonnes gardées   | Encoding |
 --- | --- | 
Amt( amount ) | Log (numpy) |

Age ( de la personne au moment du transaction ) |  Log (numpy) |

Distance ( distance entre le commerçant et le titulaire de la carte ) |  Log (numpy) |

Category ( du commerçant ) |  One Hot Encoding |

Credit card type|  One Hot Encoding |

State | One Hot Encoding |

Day | One Hot Encoding |
 
Hour | One Hot Encoding |
 
Month | One Hot Encoding |

### Algo / Modele ###

# RANDOM FOREST # and # RÉSEAU DE NEURONES CLASSIFIER ARTIFICIELS # 

# Random Forest Classifier #
• n_estimators = 100
• Validation croisée
• 4/5 pour l’apprentissage et 1/5 pour la validation à chaque fois
• Métriques: • Precision
• Recall
• F1-score

# Réseau De Neurones #
• Une seule couche cachée (34 nn) avec un dropout de 0.5.
• Fonctions d’activations : relu -> relu -> softmax
• Adam optimizer avec un pas de 0.001
• Fonctions loss :
sparse_categorical_crossentropy
• Batch = 150
• Epochs = 50
Résultats Graphes d’apprentissage :
