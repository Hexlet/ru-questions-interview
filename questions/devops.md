## Вопросы для DevOps-инженеров

* Приходилось самостоятельно писать Dockerfile? Чем отличается команда `ADD` от `COPY`?
* Для чего нужны `CMD`, `ENTRYPOINT`?
* В Docker есть понятие слоев. Что это такое?
* В слой делаем `run yum update`. Как Docker понимает что нужно пересобирать кэш, сбросить кэш или он `yum update` один раз сделал и больше делать его не будет?
* В Docker есть понятие multi-stage? Что это такое, зачем используется?
* Команда `COPY . .` Хотим все что у нас в корне скопировать в корень контейнера. Мы можем ограничить что будет копироваться? В Dockerfile не меняем ничего.
* Как посмотреть логи работающего контейнера? Как посмотреть определённое количество строк лога?
* Допустим, есть файл с логами. Там Warning, INFO, ERROR и так далее. Как посмотреть только ошибки в файле лога? Как посмотреть саму ошибку и 10 строчек до и после неё?
* Как попасть в bash работающего контейнера?
* Приходилось работать с volume в Docker?
* Мы можем примонтировать директорию к контейнеру, а можем указать "используй такой-то volume". В чем разница?
* Приходилось работать с пайплайнами Gitlab Runner? Какие виды пайплайнов есть?
* Необходимо отследить путь от одного хоста к другому, какой командой можно это сделать?
* Что такое TTL?
* У меня есть клиент-сервер. Как замерить пропускную способность между клиентом и сервером, какой командой?
* TCP и UDP, в чем отличия? За счёт чего и какие гарантии доставки?
* Клиент что-то отправляет на сервер. Во время соединения был перезагружен роутер. Будет ли доставлен пакет после перезагрузки роутера? В течение какого времени возможна доставка?
* Отличия HTTP и HTTPS. Плюсы HTTPS помимо шифрования. За счёт чего нельзя просто подменить запрашиваемый сайт. HTTP это текстовый или бинарный протокол?
* Сталкивался с REST? Какие методы есть, чем отличаются, когда используются? Основные 5. Отличия GET и POST.
* URL при использовании HTTPS зашифрован? Если взять POST, то в URL мы можем передать информацию?
* Basic auth. Что это такое и как оно передаёт свои данные?
* Есть URL, тело запроса. Что еще передается при запросе?
* Какие типы http-заголовков знаешь?
* У нас есть какой-то диск, который хотим примонтировать в Linux. Как это можно сделать? Останется ли примонтирован диск после перезагрузки при монтировании командой `mount`. Опции монтирования `fstab` - какие есть, зачем нужны?
* Метрики. `I/O wait time` - что оно показывает? Как проверить загруженность диска? Как посмотреть количество свободной оперативной памяти?
* Команда `free` - отличия столбцов free от available. Что показывают остальные столбцы?
