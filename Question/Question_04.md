# Закріплення матеріалу

## • Що таке docker-compose файл
Docker Compose файл (`docker-compose.yml`) - це конфігураційний файл у форматі YAML, що використовується для визначення багатоконтейнерних Docker-додатків. Він описує сервіси, які необхідно запустити, їх налаштування, мережі, томи та змінні оточення.

## • Що таке сервіс у docker-compose
Сервіс у Docker Compose - це окремий контейнер або група контейнерів, які виконують певну роль у додатку. Кожен сервіс має свої налаштування, такі як образ, порти, змінні оточення та інші параметри, що визначають його поведінку.

## • Якою командою можна запустити docker-compose
Запуск Docker Compose здійснюється за допомогою команди `docker-compose up`. Ця команда створює та запускає всі сервіси, визначені у файлі `docker-compose.yml`.

## • Для чого потрібна оркестрація
Окрестрація необхідна для автоматизації розгортання, управління та масштабування контейнерних додатків. Вона забезпечує управління ресурсами, моніторинг стану контейнерів, балансування навантаження та забезпечення високої доступності додатків.

## • Що таке Docker Swarm
Docker Swarm - це вбудована система оркестрації контейнерів у Docker, яка дозволяє створювати та керувати кластерами Docker-хостів. Вона забезпечує автоматичне масштабування, високу доступність, балансування навантаження та відновлення контейнерів у разі відмови.
