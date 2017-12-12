# Требования

## Требования пользователя

### Программные интерфейсы

- Авторизация пользователей должена быть возможена через следующие сервисы:
  - ВК
  - Facebook
  - Google
  - GitHub
- Должно быть реализовано REST и SOAP API, позволяющее полноценно работать с приложением, в том числе от лица администратора. 

### Интерфейс пользователя

- Главный экран приложения
  ![Main](mockups/Main.png)
- Кабинет пользователя
  ![PersonalPage](mockups/Personal.png)
- Страница с очередью
  ![QueuePage](mockups/QueuePage.png)

### Характеристики пользователей

QueueBrain хорошо подойдет для огранизации нерегулярных очередей с несложными процессами обработки. Интерфейс и идея программы достаточно просты и привычны для среднего Интернет-пользоватлея.

## Системные требования:

#### Управление пользователями

- Зарегестрированные пользователи должны иметь возможность:
  - Вставать в очереди
  - Выходить из очереди
  - Создавать очереди и управлять ими
  - Оставлять комментарии к очереди
- Незарегестрированные пользователи также должны иметь возможность встать в очередь, если это разрешено администратором. 
- Пользователи должны иметь возможность оставить в приложении данные для связи.
- Пользователь должен иметь возможность управлять оповещаниями от приложения.

#### Управление очередями

- Доступ к управлению очередью должен иметь только администратор. 

- При создании очереди должны быть доступны следующие настройки:

  - Название очереди

  - Доступность очереди незарегестрированным пользователям

  - Лимит на участников очереди (если есть)

    ![](mockups/createQueuePopup.png)

- Администратор должен иметь возможность управлять продвижением очереди:
  - Перейти к следующему пользователю
  - Изменить состояние очереди (не начата/активна/пауза/завершена)

- На иформационной странице очереди должна быть доступна информация:
  - Состояние очереди (не начата/активна/пауза/завершена)
  - Среднее время обработки
  - QR-код ссылки на очередь
  - Последний обработанный пользователь и количество ожидающих пользователей

#### Управление профилем

На вкладке управления профилем должны быть доступны следующие настройки:

* Контактные данные. Текстовое поле с любой информацией

* Включение/выключение email-нотификации о приближении очереди

* Удаление аккаунта

  ![](mockups/editProfileTab.png)

Для просмотра должна быть доступна следующая информация:

* Имя пользователя
* Контактные данные (зависит от способа регистрации)

#### Использование очереди

- При регистрации в очереди пользователь должен получить свой уникальный код. 
- Администратору при обработке пользователя должен быть доступен его уникальный код.

### Нефункциональные требования

- Приложение должно работать по защищенному протоколу.
- Приложение должно быть интернационализованным (поддержка как минимум русского и английского языков).

## Аналоги

Основное отличие от большинства аналогов -- способ предоставления сервиса. QueueBrain является веб-приложением, это значительно упрощает процесс использования, а публичное API позволяет легко интегрировать его с другими системами. 
Все перечисленные аналоги требуют предварительной установки и настройки.

- https://led-displays.ru/programma_suo.html
  - Платная
  - Сервер очереди должен находиться локальной сети
  - Windows only
- http://www.kkc.by/katalog/spec-sistemy/sistema-upravleniya-ocheredyu
  - Платная
- http://apertum.com.ua/
  - Сервер очереди должен находиться локальной сети
