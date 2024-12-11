
# Домашнее задание к занятию 5 «Тестирование roles»

## Molecule

При запуске molecule test -s ubuntu_xenial для clickhouse видим следующие результаты:

![alt text](image-7.png)

При запуске molecule test для Vector видим следующие результаты:

Роль Destroy

![alt text](image-1.png)

Создание тестовой среды

![alt text](image-2.png)

Развертывание роли в тестовую среду

![alt text](image-3.png)

Тест на идемпотентность

![alt text](image-4.png)

Тест verify

![alt text](image-5.png)

Очистка тестовой среды

![alt text](image-6.png)




## Итог

[Репозиторий Vector](https://github.com/gaidarvu/vector-role/tree/v1.1.0)

[Репозиторий LightHouse](https://github.com/gaidarvu/lighthouse-role/tree/v1.2.1)

[Репозиторий Nginx](https://github.com/gaidarvu/nginx-role/tree/v1.1.0)

[Финальный код (ссылка на репозиторий)](https://github.com/gaidarvu/ansible-netology/tree/hw-ansible-04/hw-ansible-02/playbook)