# Colab_GAN

Der Code wurde in Google Colab geschrieben. Er implementiert ein einfaches GAN.
Quelle 28 empfiehlt Dropoutrate für D=[0.4,0.7]
                                    G=[0.3,0.5]
und als Aktivierungsfunktion für D und G: ReLU und Sigmoid.

Test 1:
Dropout Generator: 0.3
Dopout Discriminator: 0.4
BatchNormalization(momentum=0.9)
ActivationFunktion Generator: LeakyReLU und Sigmoid
ActivationFunktion Discriminator: LeakyReLU und Sigmoid
Optimizer: ADAM

Test 2: (anders: ActivationFunktion und Momentum)
Dropout Generator: 0.3
Dopout Discriminator: 0.4
BatchNormalization(momentum=0.99)
ActivationFunktion Generator: LeakyReLU und Softmax
ActivationFunktion Discriminator: LeakyReLU und Softmax
Optimizer: ADAM
Funktion generate_and_save_image() Aufruf model() zu generator() geändert.
