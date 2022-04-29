# tp-lab07

https://github.com/roflanpotsan/factorial

https://github.com/roflanpotsan/hunter

1. Создать репозиторий для пакета, который можно будет подключать через Hunter.
2. Написать код, [CMakeLists.txt](https://github.com/hunterbox/hunter_box_1/blob/master/CMakeLists.txt) и [Config.cmake.in](https://github.com/hunterbox/hunter_box_1/blob/master/cmake/Config.cmake.in) .
3. Спушить с тегом, который будет являться параметром VERSION в hunter.cmake .
4. Сделать форк hunter'а и добавить в hunter/cmake/projects папку с проектом, ее название будет использоваться при добавлении проекта через hunter.
5. Создать в ней файл hunter.cmake и заполнить согласно инструкциям, указанным [здесь](https://hunter.readthedocs.io/en/latest/creating-new/create/cmake.html#add-versions). Стоит обратить внмание на пункт [Consistency](https://hunter.readthedocs.io/en/latest/creating-new/create/cmake.html#consistency). Как генерировать SHA1 указанно в инструкции по заполнению hunter.cmake
6. Пушим наш форк с тегом.
7. Создаем проект к которому хотим подключить наш пакет, добавляем туда HunterGate.cmake, который можно взять [здесь](https://github.com/cpp-pm/gate).
8. Заполняем CMakeLists.txt согласно [примеру](https://hunter.readthedocs.io/en/latest/quick-start/boost-components.html), но ссылку указываем на наш форк и генерим хеш именно для него.
9. Готово 😎
