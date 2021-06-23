# Unity-Gesture-Recognizer
Пример небольшого тестового проекта, реализующего классификацию изображений с помощью нейросети на основе TensorFlow и алгоритм $Q для Unity HDRP.

## Runes
<p align="center"> 
   <img src="https://user-images.githubusercontent.com/56678785/120069927-e6d63e00-c0a1-11eb-8329-31bf9b0eca37.png">
</p>

## [Билд проекта под Window](https://disk.yandex.ru/d/-ZuyfOGqckKD8A)

## TensorFlow
Так как до этого я не работал с нейронными сетями, была использована нейросеть для распознания цифр от 0 до 9, примеры реализации которой легко можно найти в интернете. Изначально планировалось переобучить нейросеть на распознание рун в конце разработки проекта, но, так как время, которое в итоге нейросеть тратила на распознание изображения 28x28 пикселей, было примерно равно 2-3 секундам, было решено отказаться от её использования. Нейросеть по-прежнему доступна в проекте, она работает, но распознает только цифры от 1 до 9, три группы рун.

## $Q Super-Quick Recognizer
Это 5 версия алгоритма семейства $, предназначенного для быстрого распознания жестов на маломощных устройствах. Главными преимуществами данного алгоритма являются скорость работы, около 10-20 мс, и малое потребление ресурсов устройства. К сожалению, в проекте он не всегда правильно распознает нарисованную руну, так как я сделал мало данных для сравнения, по 5 примеров на каждую рунну. Оптимально примерно по 10 прримеров на руну, плюс было бы хорошо, чтобы их делало несколько человек, чтобы было больше разницы в написание.

## Итог
Несмотря на то, что в финале используется алгоритм $Q, а текущую реализацию TensorFlow надо полностью удалить(как минимум по тому, что для этого использовались устаревшие библиотеки из пакета ML-Agent), в будущем все же хочу использовать нейросеть. Надо будет изучить материалы по ним, изучить пакет ML-Agent, и реализовать новую нейросеть.
