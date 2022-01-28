Ford vs Ferrari: определяем модель авто по фото

Модели показывают хороший результат при адекватном количестве эпох и более высоком разрешении фотографий
Для повышения качества нейронной сети был пременён метод transfer-learning
Хороший результат показала сеть EfficientNet B3
Также для повышения качества сети была применена аугментация данных с помощью ImageDataGenerator
Для улучшения предсказаний на сабмите применён Test-time augmentations (TTA).

Для улучшения модели возможны следующие пути решения:
Применение transfer learning с fine-tuning
Настройка LR, optimizer, loss
Подбор других переменных (размер картинки, батч и т.д.)
Использование иных архитектур сетей (а не только Xception) или их ансамбли. Примеры SOTA на ImageNet
Использование Batch Normalization и настройка архитектуры “головы”
Применение других функций callback Keras https://keras.io/callbacks/
Использование разных техник управления Learning Rate (https://towardsdatascience.com/finding-good-learning-rate-and-the-one-cycle-policy-7159fe1db5d6 (eng) http://teleported.in/posts/cyclic-learning-rate/ (eng))
Использование более продвинутых библиотек аугментации изображений (например, Albumentations)