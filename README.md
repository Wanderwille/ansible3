# Домашнее задание к занятию 3 «Использование Ansible» - Подус Сергей

## Основная часть

1. Допишите playbook: нужно сделать ещё один play, который устанавливает и настраивает LightHouse.
2. При создании tasks рекомендую использовать модули: `get_url`, `template`, `yum`, `apt`.
3. Tasks должны: скачать статику LightHouse, установить Nginx или любой другой веб-сервер, настроить его конфиг для открытия LightHouse, запустить веб-сервер.
4. Подготовьте свой inventory-файл `prod.yml`.
5. Запустите `ansible-lint site.yml` и исправьте ошибки, если они есть.
6. Попробуйте запустить playbook на этом окружении с флагом `--check`.
7. Запустите playbook на `prod.yml` окружении с флагом `--diff`. Убедитесь, что изменения на системе произведены.
8. Повторно запустите playbook с флагом `--diff` и убедитесь, что playbook идемпотентен.
9. Подготовьте README.md-файл по своему playbook. В нём должно быть описано: что делает playbook, какие у него есть параметры и теги.
10. Готовый playbook выложите в свой репозиторий, поставьте тег `08-ansible-03-yandex` на фиксирующий коммит, в ответ предоставьте ссылку на него.

---

# Ответ:

4. Файл prod.yaml 

![Скриншот 1](https://github.com/Wanderwille/scrinshot/blob/main/ansible3-prod.png)

5. Запуск ansible-lint (были ошибки с использованием true или false(Которое им не являлось), так же была ошибка с отсутствием символа новой строки)

![Скриншот 2](https://github.com/Wanderwille/scrinshot/blob/main/ansible-3linat-up.png)

![Скриншот 3](https://github.com/Wanderwille/scrinshot/blob/main/ansible3-ispr.png)

6. Запуск с флагом `--check`

![Скриншот 4](https://github.com/Wanderwille/scrinshot/blob/main/ansible3-check.png)

7. Запуск с флагом `--diff`

![Скриншот 5](https://github.com/Wanderwille/scrinshot/blob/main/ansible3-diff.png)

![Скриншот 5](https://github.com/Wanderwille/scrinshot/blob/main/ansible3-diff2.png)

8. Повторый запуск с флагом `--diff`

![Скриншот 5](https://github.com/Wanderwille/scrinshot/blob/main/ansible3-diff(повторный).png)

9. Ссылка на файл README.md: https://github.com/Wanderwille/ansible3/blob/main/scr/README.MD