# Домашнее задание к занятию "`Репликация и масштабирование. Часть 1`" - `Тимохин Максим`

Задание можно выполнить как в любом IDE, так и в командной строке.

### Задание 1

На лекции рассматривались режимы репликации master-slave, master-master, опишите их различия.

*Разница в том, куда можно писать данные. В master-slave писать можно только на один главный сервер (master), а подчинённые (slave) только читают и копируют данные с него. В master-master оба сервера равны: можно писать на любой, и изменения будут копироваться на другой.*

---

### Задание 2

Выполните конфигурацию master-slave репликации, примером можно пользоваться из лекции.

*1. Проверяем статус на мастере*
<img width="723" height="528" alt="image" src="https://github.com/user-attachments/assets/864654bd-166f-4290-a85c-33e1967797b2" />

*2. Проверяем статус на слейве*
<img width="744" height="629" alt="image" src="https://github.com/user-attachments/assets/f3d92553-1039-440d-9380-9b9411ddf946" />

*3. Создаём новую БД на мастере*

<img width="678" height="647" alt="image" src="https://github.com/user-attachments/assets/5118654d-5e74-47f9-8c6d-c207a96be4dd" />

*4. Проверяем, что она появилась на слейве*
<img width="679" height="702" alt="image" src="https://github.com/user-attachments/assets/80ca8b21-f694-4e57-9ff5-2a3ca4b2e327" />

*5. Пытаемся создать новую БД на слейве и убеждаемся в ограничении прав*
<img width="1255" height="661" alt="image" src="https://github.com/user-attachments/assets/d94f090e-b857-418f-9d2e-8df06695e44d" />
