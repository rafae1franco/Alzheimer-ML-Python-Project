# Alzheimer-ML-Python-Project
Modelo de Rede Neural com TensorFlow para Previsão de Alzheimer

Este projeto tem como objetivo a classificação de imagens para previsão da doença de Alzheimer utilizando uma Rede Neural Convolucional (CNN) com TensorFlow e Keras. (Uma CNN é um tipo de inteligência artificial que aprende a reconhecer padrões em imagens, como os que aparecem em exames médicos.) O modelo foi treinado com um conjunto de imagens de ressonância magnética contidas no dataset "Alzheimer Dataset".

Funcionalidades:

Carregamento e Processamento dos Dados: O dataset é extraído do Google Drive e suas imagens são carregadas utilizando a classe ImageDataGenerator, que também aplica técnicas de aumento de dados, como redimensionamento (ajustar tamanho), zoom (aproximar a imagem) e inversão horizontal (espelhar a imagem para melhor aprendizado do modelo).

Treinamento e Avaliação: O modelo de CNN é treinado com imagens de diferentes classes (Normal, Mild Demented, Moderate Demented e Very Mild Demented), utilizando a função de perda categorical_crossentropy (mede o erro do modelo) e o otimizador adam (ajusta os pesos do modelo para melhorar a precisão).

Matriz de Confusão: Após o treinamento, a performance do modelo é avaliada através da matriz de confusão (uma tabela que mostra quantas previsões o modelo acertou e errou), permitindo a análise da precisão para cada classe.

Classificação de Novas Imagens: Foi implementada uma função personalizada que permite a previsão do diagnóstico a partir de uma nova imagem de entrada, exibindo-a juntamente com a classe prevista.

Arquitetura do Modelo:

Camadas convolucionais Conv2D seguidas de MaxPooling2D para extração de padrões visuais (essas camadas ajudam a destacar as características mais importantes da imagem).

Camadas totalmente conectadas Dense com ativação relu para aprendizado complexo (ajudam o modelo a entender relações mais sofisticadas nos dados).

Camada de saída com ativação sigmoid para classificação multiclasse (gera a probabilidade de cada classe, ajudando o modelo a decidir qual diagnóstico é mais provável).

Este projeto foi desenvolvido como parte da disciplina de Tópicos Avançados - INF 2024, sob a orientação do professor Antonio Queiroz da Silva Neto.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# Alzheimer-ML-Python-Project
Neural Network Model with TensorFlow for Alzheimer Prediction

This project aims to classify images to predict Alzheimer’s disease using a Convolutional Neural Network (CNN) with TensorFlow and Keras. (A CNN is a type of artificial intelligence that learns to recognize patterns in images, such as those found in medical scans.) The model was trained using a set of magnetic resonance images from the "Alzheimer Dataset."

Features:

Data Loading and Processing: The dataset is extracted from Google Drive, and its images are loaded using the ImageDataGenerator class, which also applies data augmentation techniques such as resizing (adjusting size), zooming (magnifying the image), and horizontal flipping (mirroring the image to improve model learning).

Training and Evaluation: The CNN model is trained with images from different classes (Normal, Mild Demented, Moderate Demented, and Very Mild Demented), using the categorical_crossentropy loss function (measures the model’s error) and the adam optimizer (adjusts the model’s weights to improve accuracy).

Confusion Matrix: After training, the model's performance is evaluated using a confusion matrix (a table that shows how many predictions the model got right and wrong), allowing an analysis of accuracy for each class.

New Image Classification: A custom function has been implemented to predict the diagnosis based on a new input image, displaying it along with the predicted class.

Model Architecture:

Conv2D convolutional layers followed by MaxPooling2D for feature extraction (these layers help highlight the most important characteristics in the image).

Fully connected Dense layers with relu activation for complex learning (help the model understand more sophisticated relationships in the data).

Output layer with sigmoid activation for multi-class classification (generates the probability of each class, helping the model determine the most likely diagnosis).

This project was developed as part of the Advanced Topics - INF 2024 course, under the guidance of Professor Antonio Queiroz da Silva Neto.



