
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


## Tox

Запуск tox происходит по сценарию: destroy --> create --> converge --> destroy
Тестовая среда driver: podman, image: python:latest

Запуск tox, роль destroy

![alt text](image-8.png)

Роль create

![alt text](image-9.png)

Роль converge

![alt text](image-10.png)

Роль destroy + info

![alt text](image-11.png)

## Итог

[Репозиторий с тегом Molecule](https://github.com/gaidarvu/ansible-netology/tree/v1.0.0)

[Репозиторий с тегом Tox](https://github.com/gaidarvu/ansible-netology/tree/tox1.0.1)

[Финальный код (ссылка на репозиторий)](https://github.com/gaidarvu/ansible-netology/tree/hw-ansible-05)