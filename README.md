Стэк работоает с любыми типами, для работы ему необходимо иметь метод operator<< для std::ostream. Яд - побайтовый. В конце каждой операции (создание, присваивание, push, pop) происходит dump в log.txt. Информация о кодах ошибок выводится в log.txt, на экран выводится только информация об их наличии. Программа падает только в одном случае - если не удалось выделить память под data. Код ошибки в этом случае - 1. Также на экран выводятся некоторые предупреждения (если запрошен стэк с отрицательным или нулевым числом элементов, если есть попытка вытащить элемент из пустого стэка (в этом случае всегда возвращается нулевой элемент), если log.txt не получилось открыть). Хэш, вероятно, так себе
