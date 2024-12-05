
# Домашнее задание к занятию 4 «Работа с roles»

## Описание
Данный playbook выполняет развертывание в Yandex Cloud:

При помощи ansible-galaxy вытягиваем роли с нужными версиями из гита, указанные в requirements.yml

Поскольку для раскатки LightHouse необходим nginx, вытянул его роль из гита таким-же образом, как и все остальные роли и включил в LightHouse как include_role

Можно было сделать и таким образом:

```yaml
- name: Install LightHouse
  become: true
  hosts: lighthouse
  roles:
    - nginx
    - lighthouse
```
Playbook является идемпотентным

![alt text](image.png)

## Итог

[Репозиторий Vector](https://github.com/gaidarvu/vector-role/tree/v1.1.0)

[Репозиторий LightHouse](https://github.com/gaidarvu/lighthouse-role/tree/v1.2.1)

[Репозиторий Nginx](https://github.com/gaidarvu/nginx-role/tree/v1.1.0)

[Финальный код (ссылка на репозиторий)](https://github.com/gaidarvu/ansible-netology/tree/hw-ansible-04/hw-ansible-02/playbook)