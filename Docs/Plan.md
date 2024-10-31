План выполнения работы по автоматизации тестирования

Позитивные сценарии:

Сценарий 1. Заполнение формы «Кредит по данным карты» со статусом карты «APPROVED»
Нажать на кнопку «Купить в кредит».
Заполнить поля формы «Кредит по данным карты» валидными значениями:
Номер карты со статусом «APPROVED» (например: 5555 5555 5555 5556).
Номер месяца: цифры от 01 до 12 (например: 07).
Год: две последние цифры текущего или будущего года (например: 27).
Владелец: имя на латинице (например: Elena Ivanova).
CVC/CVV: трёхзначный код (например: 456).
Нажать на кнопку «Продолжить».
Ожидаемый результат: Появление сообщения об успешной операции. Форма успешно отправлена. В базе данных регистрируется новая транзакция со статусом "APPROVED".
Сценарий 2. Заполнение формы «Оплата по карте» со статусом карты «DECLINED»
Нажать на кнопку «Купить».
Заполнить поля формы «Оплата по карте» валидными значениями:
Номер карты со статусом «DECLINED» (например: 5555 5555 5555 5550).
Номер месяца: цифры от 01 до 12 (например: 10).
Год: две последние цифры текущего или будущего года (например: 26).
Владелец: имя на латинице (например: Sergey Petrov).
CVC/CVV: трёхзначный код (например: 321).
Нажать на кнопку «Продолжить».
Ожидаемый результат: Появление сообщения об отклонении операции. Форма не отправлена. В базе данных регистрируется новая транзакция со статусом "DECLINED".
Сценарий 3. Заполнение формы «Оплата по карте» со статусом карты «APPROVED»
Нажать на кнопку «Купить».
Заполнить поля формы «Оплата по карте» валидными значениями:
Номер карты со статусом «APPROVED» (например: 4111 1111 1111 1118).
Номер месяца: цифры от 01 до 12 (например: 03).
Год: две последние цифры текущего или будущего года (например: 24).
Владелец: имя на латинице (например: Olga Smirnova).
CVC/CVV: трёхзначный код (например: 789).
Нажать на кнопку «Продолжить».
Ожидаемый результат: Появление сообщения об успешной операции. Форма успешно отправлена. В базе данных регистрируется новая транзакция со статусом "APPROVED".
Сценарий 4. Заполнение формы «Кредит по данным карты» со статусом карты «DECLINED»
Нажать на кнопку «Купить в кредит».
Заполнить поля формы «Кредит по данным карты» валидными значениями:
Номер карты со статусом «DECLINED» (например: 4111 1111 1111 1115).
Номер месяца: цифры от 01 до 12 (например: 11).
Год: две последние цифры текущего или будущего года (например: 28).
Владелец: имя на латинице (например: Igor Sokolov).
CVC/CVV: трёхзначный код (например: 654).
Нажать на кнопку «Продолжить».
Ожидаемый результат: Появление сообщения об отклонении операции. Форма не отправлена. В базе данных регистрируется новая транзакция со статусом "DECLINED".

Негативные сценарии Формы «Оплата по карте»:

Сценарий 1. Заполнение поля «Номер карты» номером, состоящим из 1 цифры
Кликнуть на кнопку «Купить»
Ввести в поле «Номер карты» номер, состоящий из 1 цифры (например: 2)
Заполнить поля «Номер месяца», «Год», «Владелец», «CVC/CVV» валидными значениями
Кликнуть на кнопку «Продолжить»
Ожидаемый результат: Появление сообщения об ошибке «Неверный формат» в поле «Номер карты». Форма не отправлена
Сценарий 2. Заполнение поля «Номер карты» номером, состоящим из 2 цифр
Кликнуть на кнопку «Купить»
Ввести в поле «Номер карты» номер, состоящий из 2 цифр (например: 21)
Заполнить поля «Номер месяца», «Год», «Владелец», «CVC/CVV» валидными значениями
Кликнуть на кнопку «Продолжить»
Ожидаемый результат: Появление сообщения об ошибке «Неверный формат» в поле «Номер карты». Форма не отправлена
Сценарий 3. Заполнение поля «Номер карты» номером, состоящим из 15 цифр
Кликнуть на кнопку «Купить»
Ввести в поле «Номер карты» номер, состоящий из 15 цифр (например: 4444 4444 4444 444)
Заполнить поля «Номер месяца», «Год», «Владелец», «CVC/CVV» валидными значениями
Кликнуть на кнопку «Продолжить»
Ожидаемый результат: Появление сообщения об ошибке «Неверный формат» в поле «Номер карты». Форма не отправлена
Сценарий 4. Заполнение поля «Номер карты» номером, состоящим из 17 цифр
Кликнуть на кнопку «Купить»
Ввести в поле «Номер карты» номер, состоящий из 17 цифр (например: 4444 4444 4444 4441 4)
Заполнить поля «Номер месяца», «Год», «Владелец», «CVC/CVV» валидными значениями
Кликнуть на кнопку «Продолжить»
Ожидаемый результат: Появление сообщения об ошибке «Неверный формат» в поле «Номер карты». Форма не отправлена
Сценарий 5. Заполнение поля «Номер карты» специальными символами
Кликнуть на кнопку «Купить»
Ввести в поле «Номер карты» специальные символы (например: @#&)
Заполнить поля «Номер месяца», «Год», «Владелец», «CVC/CVV» валидными значениями
Кликнуть на кнопку «Продолжить»
Ожидаемый результат: Появление сообщения об ошибке «Неверный формат» в поле «Номер карты». Форма не отправлена
Сценарий 6. Заполнение поля «Номер карты» значением на кириллице
Кликнуть на кнопку «Купить»
Ввести в поле «Номер карты» значение на кириллице (например: номер)
Заполнить поля «Номер месяца», «Год», «Владелец», «CVC/CVV» валидными значениями
Кликнуть на кнопку «Продолжить»
Ожидаемый результат: Появление сообщения об ошибке «Неверный формат» в поле «Номер карты». Форма не отправлена
Сценарий 7. Заполнение поля «Номер карты» значением на латинице
Кликнуть на кнопку «Купить»
Ввести в поле «Номер карты» значение на латинице (например: number)
Заполнить поля «Номер месяца», «Год», «Владелец», «CVC/CVV» валидными значениями
Кликнуть на кнопку «Продолжить»
Ожидаемый результат: Появление сообщения об ошибке «Неверный формат» в поле «Номер карты». Форма не отправлена
Сценарий 8. Не заполнение поля «Номер карты»
Кликнуть на кнопку «Купить»
Оставить поле «Номер карты» пустым
Заполнить поля «Номер месяца», «Год», «Владелец», «CVC/CVV» валидными значениями
Кликнуть на кнопку «Продолжить»
Ожидаемый результат: Появление сообщения об ошибке «Неверный формат» в поле «Номер карты». Форма не отправлена
Сценарий 9. Заполнение поля «Месяц» несуществующим месяцем, в пределах граничных значений
Кликнуть на кнопку «Купить»
Ввести в поле «Месяц» несуществующий месяц в пределах граничных значений цифрами, вне диапазона от 01 до 12 (например: 13)
Заполнить поля «Номер карты», «Год», «Владелец», «CVC/CVV» валидными значениями
Кликнуть на кнопку «Продолжить»
Ожидаемый результат: Появление сообщения об ошибке «Неверно указан срок действия карты» в поле «Месяц». Форма не отправлена
Сценарий 10. Заполнение поля «Месяц» значением равным двум нулям
Кликнуть на кнопку «Купить»
Ввести в поле «Месяц» значение равное двум нулям (например: 00)
Заполнить поля «Номер карты», «Год», «Владелец», «CVC/CVV» валидными значениями
Кликнуть на кнопку «Продолжить»
Ожидаемый результат: Появление сообщения об ошибке «Неверно указан срок действия карты» в поле «Месяц». Форма не отправлена
Сценарий 11. Заполнение поля «Месяц» значением из 3 цифр
Кликнуть на кнопку «Купить»
Ввести в поле «Месяц» значение из 3 цифр (например: 123)
Заполнить поля «Номер карты», «Год», «Владелец», «CVC/CVV» валидными значениями
Кликнуть на кнопку «Продолжить»
Ожидаемый результат: Появление сообщения об ошибке «Неверно указан срок действия карты» в поле «Месяц». Форма не отправлена
Сценарий 12. Заполнение поля «Месяц» значением из 1 цифры
Кликнуть на кнопку «Купить»
Ввести в поле «Месяц» значение из 1 цифры (например: 4)
Заполнить поля «Номер карты», «Год», «Владелец», «CVC/CVV» валидными значениями
Кликнуть на кнопку «Продолжить»
Ожидаемый результат: Появление сообщения об ошибке «Неверный формат» в поле «Месяц». Форма не отправлена
Сценарий 13. Заполнение поля «Месяц» специальными символами
Кликнуть на кнопку «Купить»
Ввести в поле «Месяц» специальные символы (например: @#)
Заполнить поля «Номер карты», «Год», «Владелец», «CVC/CVV» валидными значениями
Кликнуть на кнопку «Продолжить»
Ожидаемый результат: Появление сообщения об ошибке «Неверный формат» в поле «Месяц». Форма не отправлена
Сценарий 14. Заполнение поля «Год» значением прошедшего года
Кликнуть на кнопку «Купить»
Ввести в поле «Год» значение прошедшего года (например: 21)
Заполнить поля «Номер карты», «Месяц», «Владелец», «CVC/CVV» валидными значениями
Кликнуть на кнопку «Продолжить»
Ожидаемый результат: Появление сообщения об ошибке «Истёк срок действия карты» в поле «Год». Форма не отправлена
Сценарий 15. Заполнение поля «Год» значением, на 25 лет превышающего текущий год
Кликнуть на кнопку «Купить»
Ввести в поле «Год» значение, на 25 лет превышающее текущий год (например: 50)
Заполнить поля «Номер карты», «Месяц», «Владелец», «CVC/CVV» валидными значениями
Кликнуть на кнопку «Продолжить»
Ожидаемый результат: Появление сообщения об ошибке «Неверно указан срок действия карты» в поле «Год». Форма не отправлена
Сценарий 16. Заполнение поля «Год» значением из 1 цифры
Кликнуть на кнопку «Купить»
Ввести в поле «Год» значение из 1 цифры (например: 3)
Заполнить поля «Номер карты», «Месяц», «Владелец», «CVC/CVV» валидными значениями
Кликнуть на кнопку «Продолжить»
Ожидаемый результат: Появление сообщения об ошибке «Неверный формат» в поле «Год». Форма не отправлена
Сценарий 17. Заполнение поля «Год» значением из 3 цифр
Кликнуть на кнопку «Купить»
Ввести в поле «Год» значение из 3 цифр (например: 203)
Заполнить поля «Номер карты», «Месяц», «Владелец», «CVC/CVV» валидными значениями
Кликнуть на кнопку «Продолжить»
Ожидаемый результат: Появление сообщения об ошибке «Неверный формат» в поле «Год». Форма не отправлена
Сценарий 18. Заполнение поля «Год» значением, равным нулю
Кликнуть на кнопку «Купить»
Ввести в поле «Год» значение равное нулю (например: 0)
Заполнить поля «Номер карты», «Месяц», «Владелец», «CVC/CVV» валидными значениями
Кликнуть на кнопку «Продолжить»
Ожидаемый результат: Появление сообщения об ошибке «Неверный формат» в поле «Год». Форма не отправлена
Сценарий 19. Заполнение поля «Год» специальными символами
Кликнуть на кнопку «Купить»
Ввести в поле «Год» специальные символы (например: !@#)
Заполнить поля «Номер карты», «Месяц», «Владелец», «CVC/CVV» валидными значениями
Кликнуть на кнопку «Продолжить»
Ожидаемый результат: Появление сообщения об ошибке «Неверный формат» в поле «Год». Форма не отправлена
Сценарий 20. Заполнение поля «Владелец» значением из 1 буквы
Кликнуть на кнопку «Купить»
Ввести в поле «Владелец» значение из 1 буквы (например: A)
Заполнить поля «Номер карты», «Месяц», «Год», «CVC/CVV» валидными значениями
Кликнуть на кнопку «Продолжить»
Ожидаемый результат: Появление сообщения об ошибке «Неверное имя» в поле «Владелец». Форма не отправлена
Сценарий 21. Заполнение поля «Владелец» значением из 60 букв
Кликнуть на кнопку «Купить»
Ввести в поле «Владелец» значение из 60 букв (например: Александра Александровна Аааааааааааааааааааааааааааа)
Заполнить поля «Номер карты», «Месяц», «Год», «CVC/CVV» валидными значениями
Кликнуть на кнопку «Продолжить»
Ожидаемый результат: Появление сообщения об ошибке «Неверное имя» в поле «Владелец». Форма не отправлена
Сценарий 22. Заполнение поля «Владелец» значением на кириллице
Кликнуть на кнопку «Купить»
Ввести в поле «Владелец» значение на кириллице (например: Игорь Сидоров)
Заполнить поля «Номер карты», «Месяц», «Год», «CVC/CVV» валидными значениями
Кликнуть на кнопку «Продолжить»
Ожидаемый результат: Появление сообщения об ошибке «Неверное имя» в поле «Владелец». Форма не отправлена
Сценарий 23. Заполнение поля «Владелец» цифрами
Кликнуть на кнопку «Купить»
Ввести в поле «Владелец» цифры (например: 456)
Заполнить поля «Номер карты», «Месяц», «Год», «CVC/CVV» валидными значениями
Кликнуть на кнопку «Продолжить»
Ожидаемый результат: Появление сообщения об ошибке «Неверное имя» в поле «Владелец». Форма не отправлена
Сценарий 24. Заполнение поля «Владелец» специальными символами
Кликнуть на кнопку «Купить»
Ввести в поле «Владелец» специальные символы (например: $%^)
Заполнить поля «Номер карты», «Месяц», «Год», «CVC/CVV» валидными значениями
Кликнуть на кнопку «Продолжить»
Ожидаемый результат: Появление сообщения об ошибке «Неверное имя» в поле «Владелец». Форма не отправлена
Сценарий 25. Не заполнение поля «Владелец»
Кликнуть на кнопку «Купить»
Оставить поле «Владелец» пустым
Заполнить поля «Номер карты», «Месяц», «Год», «CVC/CVV» валидными значениями
Кликнуть на кнопку «Продолжить»
Ожидаемый результат: Появление сообщения об ошибке «Поле обязательно для заполнения» в поле «Владелец». Форма не отправлена
Сценарий 26. Заполнение поля «CVC/CVV» значением из 1 цифры
Кликнуть на кнопку «Купить»
Ввести в поле «CVC/CVV» значение из 1 цифры (например: 1)
Заполнить поля «Номер карты», «Месяц», «Год», «Владелец» валидными значениями
Кликнуть на кнопку «Продолжить»
Ожидаемый результат: Появление сообщения об ошибке «Неверный формат» в поле «CVC/CVV». Форма не отправлена
Сценарий 27. Заполнение поля «CVC/CVV» значением из 2 цифр
Кликнуть на кнопку «Купить»
Ввести в поле «CVC/CVV» значение из 2 цифр (например: 12)
Заполнить поля «Номер карты», «Месяц», «Год», «Владелец» валидными значениями
Кликнуть на кнопку «Продолжить»
Ожидаемый результат: Появление сообщения об ошибке «Неверный формат» в поле «CVC/CVV». Форма не отправлена
Сценарий 28. Заполнение поля «CVC/CVV» значением из 4 цифр
Кликнуть на кнопку «Купить»
Ввести в поле «CVC/CVV» значение из 4 цифр (например: 1234)
Заполнить поля «Номер карты», «Месяц», «Год», «Владелец» валидными значениями
Кликнуть на кнопку «Продолжить»
Ожидаемый результат: Появление сообщения об ошибке «Неверный формат» в поле «CVC/CVV». Форма не отправлена
Сценарий 29. Заполнение поля «CVC/CVV» значением из 5 цифр
Кликнуть на кнопку «Купить»
Ввести в поле «CVC/CVV» значение из 5 цифр (например: 12345)
Заполнить поля «Номер карты», «Месяц», «Год», «Владелец» валидными значениями
Кликнуть на кнопку «Продолжить»
Ожидаемый результат: Появление сообщения об ошибке «Неверный формат» в поле «CVC/CVV». Форма не отправлена
Сценарий 30. Не заполнение формы «Оплата по карте»
Кликнуть на кнопку «Купить»
Оставить поля «Номер карты», «Месяц», «Год», «Владелец», «CVC/CVV» пустыми
Кликнуть на кнопку «Продолжить»
Ожидаемый результат: Появление сообщений об ошибках в полях. Форма не отправлена.

Негативные сценарии Формы «Кредит по данным карты»
Сценарий 1. Заполнение поля «Номер карты» номером, состоящим из 1 цифры
Кликнуть на кнопку «Купить»
Ввести в поле «Номер карты» номер, состоящий из 1 цифры (например: 2)
Заполнить поля «Номер месяца», «Год», «Владелец», «CVC/CVV» валидными значениями
Кликнуть на кнопку «Продолжить»
Ожидаемый результат: Появление сообщения об ошибке «Неверный формат» в поле «Номер карты». Форма не отправлена
Сценарий 2. Заполнение поля «Номер карты» номером, состоящим из 2 цифр
Кликнуть на кнопку «Купить»
Ввести в поле «Номер карты» номер, состоящий из 2 цифр (например: 21)
Заполнить поля «Номер месяца», «Год», «Владелец», «CVC/CVV» валидными значениями
Кликнуть на кнопку «Продолжить»
Ожидаемый результат: Появление сообщения об ошибке «Неверный формат» в поле «Номер карты». Форма не отправлена
Сценарий 3. Заполнение поля «Номер карты» номером, состоящим из 15 цифр
Кликнуть на кнопку «Купить»
Ввести в поле «Номер карты» номер, состоящий из 15 цифр (например: 4444 4444 4444 444)
Заполнить поля «Номер месяца», «Год», «Владелец», «CVC/CVV» валидными значениями
Кликнуть на кнопку «Продолжить»
Ожидаемый результат: Появление сообщения об ошибке «Неверный формат» в поле «Номер карты». Форма не отправлена
Сценарий 4. Заполнение поля «Номер карты» номером, состоящим из 17 цифр
Кликнуть на кнопку «Купить»
Ввести в поле «Номер карты» номер, состоящий из 17 цифр (например: 4444 4444 4444 4441 4)
Заполнить поля «Номер месяца», «Год», «Владелец», «CVC/CVV» валидными значениями
Кликнуть на кнопку «Продолжить»
Ожидаемый результат: Появление сообщения об ошибке «Неверный формат» в поле «Номер карты». Форма не отправлена
Сценарий 5. Заполнение поля «Номер карты» специальными символами
Кликнуть на кнопку «Купить»
Ввести в поле «Номер карты» специальные символы (например: @#&)
Заполнить поля «Номер месяца», «Год», «Владелец», «CVC/CVV» валидными значениями
Кликнуть на кнопку «Продолжить»
Ожидаемый результат: Появление сообщения об ошибке «Неверный формат» в поле «Номер карты». Форма не отправлена
Сценарий 6. Заполнение поля «Номер карты» значением на кириллице
Кликнуть на кнопку «Купить»
Ввести в поле «Номер карты» значение на кириллице (например: номер)
Заполнить поля «Номер месяца», «Год», «Владелец», «CVC/CVV» валидными значениями
Кликнуть на кнопку «Продолжить»
Ожидаемый результат: Появление сообщения об ошибке «Неверный формат» в поле «Номер карты». Форма не отправлена
Сценарий 7. Заполнение поля «Номер карты» значением на латинице
Кликнуть на кнопку «Купить»
Ввести в поле «Номер карты» значение на латинице (например: number)
Заполнить поля «Номер месяца», «Год», «Владелец», «CVC/CVV» валидными значениями
Кликнуть на кнопку «Продолжить»
Ожидаемый результат: Появление сообщения об ошибке «Неверный формат» в поле «Номер карты». Форма не отправлена
Сценарий 8. Не заполнение поля «Номер карты»
Кликнуть на кнопку «Купить»
Оставить поле «Номер карты» пустым
Заполнить поля «Номер месяца», «Год», «Владелец», «CVC/CVV» валидными значениями
Кликнуть на кнопку «Продолжить»
Ожидаемый результат: Появление сообщения об ошибке «Неверный формат» в поле «Номер карты». Форма не отправлена
Сценарий 9. Заполнение поля «Месяц» несуществующим месяцем, в пределах граничных значений
Кликнуть на кнопку «Купить»
Ввести в поле «Месяц» несуществующий месяц в пределах граничных значений цифрами, вне диапазона от 01 до 12 (например: 13)
Заполнить поля «Номер карты», «Год», «Владелец», «CVC/CVV» валидными значениями
Кликнуть на кнопку «Продолжить»
Ожидаемый результат: Появление сообщения об ошибке «Неверно указан срок действия карты» в поле «Месяц». Форма не отправлена
Сценарий 10. Заполнение поля «Месяц» значением равным двум нулям
Кликнуть на кнопку «Купить»
Ввести в поле «Месяц» значение равное двум нулям (например: 00)
Заполнить поля «Номер карты», «Год», «Владелец», «CVC/CVV» валидными значениями
Кликнуть на кнопку «Продолжить»
Ожидаемый результат: Появление сообщения об ошибке «Неверно указан срок действия карты» в поле «Месяц». Форма не отправлена
Сценарий 11. Заполнение поля «Месяц» значением из 3 цифр
Кликнуть на кнопку «Купить»
Ввести в поле «Месяц» значение из 3 цифр (например: 123)
Заполнить поля «Номер карты», «Год», «Владелец», «CVC/CVV» валидными значениями
Кликнуть на кнопку «Продолжить»
Ожидаемый результат: Появление сообщения об ошибке «Неверно указан срок действия карты» в поле «Месяц». Форма не отправлена
Сценарий 12. Заполнение поля «Месяц» значением из 1 цифры
Кликнуть на кнопку «Купить»
Ввести в поле «Месяц» значение из 1 цифры (например: 4)
Заполнить поля «Номер карты», «Год», «Владелец», «CVC/CVV» валидными значениями
Кликнуть на кнопку «Продолжить»
Ожидаемый результат: Появление сообщения об ошибке «Неверный формат» в поле «Месяц». Форма не отправлена
Сценарий 13. Заполнение поля «Месяц» специальными символами
Кликнуть на кнопку «Купить»
Ввести в поле «Месяц» специальные символы (например: @#)
Заполнить поля «Номер карты», «Год», «Владелец», «CVC/CVV» валидными значениями
Кликнуть на кнопку «Продолжить»
Ожидаемый результат: Появление сообщения об ошибке «Неверный формат» в поле «Месяц». Форма не отправлена
Сценарий 14. Заполнение поля «Год» значением прошедшего года
Кликнуть на кнопку «Купить»
Ввести в поле «Год» значение прошедшего года (например: 21)
Заполнить поля «Номер карты», «Месяц», «Владелец», «CVC/CVV» валидными значениями
Кликнуть на кнопку «Продолжить»
Ожидаемый результат: Появление сообщения об ошибке «Истёк срок действия карты» в поле «Год». Форма не отправлена
Сценарий 15. Заполнение поля «Год» значением, на 25 лет превышающего текущий год
Кликнуть на кнопку «Купить»
Ввести в поле «Год» значение, на 25 лет превышающее текущий год (например: 50)
Заполнить поля «Номер карты», «Месяц», «Владелец», «CVC/CVV» валидными значениями
Кликнуть на кнопку «Продолжить»
Ожидаемый результат: Появление сообщения об ошибке «Неверно указан срок действия карты» в поле «Год». Форма не отправлена
Сценарий 16. Заполнение поля «Год» значением из 1 цифры
Кликнуть на кнопку «Купить»
Ввести в поле «Год» значение из 1 цифры (например: 3)
Заполнить поля «Номер карты», «Месяц», «Владелец», «CVC/CVV» валидными значениями
Кликнуть на кнопку «Продолжить»
Ожидаемый результат: Появление сообщения об ошибке «Неверный формат» в поле «Год». Форма не отправлена
Сценарий 17. Заполнение поля «Год» значением из 3 цифр
Кликнуть на кнопку «Купить»
Ввести в поле «Год» значение из 3 цифр (например: 203)
Заполнить поля «Номер карты», «Месяц», «Владелец», «CVC/CVV» валидными значениями
Кликнуть на кнопку «Продолжить»
Ожидаемый результат: Появление сообщения об ошибке «Неверный формат» в поле «Год». Форма не отправлена
Сценарий 18. Заполнение поля «Год» значением, равным нулю
Кликнуть на кнопку «Купить»
Ввести в поле «Год» значение равное нулю (например: 0)
Заполнить поля «Номер карты», «Месяц», «Владелец», «CVC/CVV» валидными значениями
Кликнуть на кнопку «Продолжить»
Ожидаемый результат: Появление сообщения об ошибке «Неверный формат» в поле «Год». Форма не отправлена
Сценарий 19. Заполнение поля «Год» специальными символами
Кликнуть на кнопку «Купить»
Ввести в поле «Год» специальные символы (например: !@#)
Заполнить поля «Номер карты», «Месяц», «Владелец», «CVC/CVV» валидными значениями
Кликнуть на кнопку «Продолжить»
Ожидаемый результат: Появление сообщения об ошибке «Неверный формат» в поле «Год». Форма не отправлена
Сценарий 20. Заполнение поля «Владелец» значением из 1 буквы
Кликнуть на кнопку «Купить»
Ввести в поле «Владелец» значение из 1 буквы (например: A)
Заполнить поля «Номер карты», «Месяц», «Год», «CVC/CVV» валидными значениями
Кликнуть на кнопку «Продолжить»
Ожидаемый результат: Появление сообщения об ошибке «Неверное имя» в поле «Владелец». Форма не отправлена
Сценарий 21. Заполнение поля «Владелец» значением из 60 букв
Кликнуть на кнопку «Купить»
Ввести в поле «Владелец» значение из 60 букв (например: Александра Александровна Аааааааааааааааааааааааааааа)
Заполнить поля «Номер карты», «Месяц», «Год», «CVC/CVV» валидными значениями
Кликнуть на кнопку «Продолжить»
Ожидаемый результат: Появление сообщения об ошибке «Неверное имя» в поле «Владелец». Форма не отправлена
Сценарий 22. Заполнение поля «Владелец» значением на кириллице
Кликнуть на кнопку «Купить»
Ввести в поле «Владелец» значение на кириллице (например: Игорь Сидоров)
Заполнить поля «Номер карты», «Месяц», «Год», «CVC/CVV» валидными значениями
Кликнуть на кнопку «Продолжить»
Ожидаемый результат: Появление сообщения об ошибке «Неверное имя» в поле «Владелец». Форма не отправлена
Сценарий 23. Заполнение поля «Владелец» цифрами
Кликнуть на кнопку «Купить»
Ввести в поле «Владелец» цифры (например: 456)
Заполнить поля «Номер карты», «Месяц», «Год», «CVC/CVV» валидными значениями
Кликнуть на кнопку «Продолжить»
Ожидаемый результат: Появление сообщения об ошибке «Неверное имя» в поле «Владелец». Форма не отправлена
Сценарий 24. Заполнение поля «Владелец» специальными символами
Кликнуть на кнопку «Купить»
Ввести в поле «Владелец» специальные символы (например: $%^)
Заполнить поля «Номер карты», «Месяц», «Год», «CVC/CVV» валидными значениями
Кликнуть на кнопку «Продолжить»
Ожидаемый результат: Появление сообщения об ошибке «Неверное имя» в поле «Владелец». Форма не отправлена
Сценарий 25. Не заполнение поля «Владелец»
Кликнуть на кнопку «Купить»
Оставить поле «Владелец» пустым
Заполнить поля «Номер карты», «Месяц», «Год», «CVC/CVV» валидными значениями
Кликнуть на кнопку «Продолжить»
Ожидаемый результат: Появление сообщения об ошибке «Поле обязательно для заполнения» в поле «Владелец». Форма не отправлена
Сценарий 26. Заполнение поля «CVC/CVV» значением из 1 цифры
Кликнуть на кнопку «Купить»
Ввести в поле «CVC/CVV» значение из 1 цифры (например: 1)
Заполнить поля «Номер карты», «Месяц», «Год», «Владелец» валидными значениями
Кликнуть на кнопку «Продолжить»
Ожидаемый результат: Появление сообщения об ошибке «Неверный формат» в поле «CVC/CVV». Форма не отправлена
Сценарий 27. Заполнение поля «CVC/CVV» значением из 2 цифр
Кликнуть на кнопку «Купить»
Ввести в поле «CVC/CVV» значение из 2 цифр (например: 12)
Заполнить поля «Номер карты», «Месяц», «Год», «Владелец» валидными значениями
Кликнуть на кнопку «Продолжить»
Ожидаемый результат: Появление сообщения об ошибке «Неверный формат» в поле «CVC/CVV». Форма не отправлена
Сценарий 28. Заполнение поля «CVC/CVV» значением из 4 цифр
Кликнуть на кнопку «Купить»
Ввести в поле «CVC/CVV» значение из 4 цифр (например: 1234)
Заполнить поля «Номер карты», «Месяц», «Год», «Владелец» валидными значениями
Кликнуть на кнопку «Продолжить»
Ожидаемый результат: Появление сообщения об ошибке «Неверный формат» в поле «CVC/CVV». Форма не отправлена
Сценарий 29. Заполнение поля «CVC/CVV» значением из 5 цифр
Кликнуть на кнопку «Купить»
Ввести в поле «CVC/CVV» значение из 5 цифр (например: 12345)
Заполнить поля «Номер карты», «Месяц», «Год», «Владелец» валидными значениями
Кликнуть на кнопку «Продолжить»
Ожидаемый результат: Появление сообщения об ошибке «Неверный формат» в поле «CVC/CVV». Форма не отправлена
Сценарий 30. Не заполнение формы «Оплата по карте»
Кликнуть на кнопку «Купить»
Оставить поля «Номер карты», «Месяц», «Год», «Владелец», «CVC/CVV» пустыми
Кликнуть на кнопку «Продолжить»
Ожидаемый результат: Появление сообщений об ошибках в полях. Форма не отправлена.
Перечень используемых инструментов с обоснованием выбора:
IntelliJ IDEA – это мощная среда разработки, поддерживающая множество языков, включая Java. Она предоставляет высокую производительность, удобные инструменты для отладки и тестирования, а также расширенные возможности для рефакторинга кода. Настраиваемый интерфейс и интеграция с современными инструментами делают её идеальным выбором для разработчиков. Активное сообщество и регулярные обновления обеспечивают стабильную поддержку и доступ к новым функциям.
Gradle – инструмент, используемый для управления зависимостями и сборки проектов, который упрощает процесс автоматизации сборки.
Docker и Docker Compose – технологии, позволяющие создавать изолированные среды с необходимыми сервисами, такими как MySQL, PostgreSQL и эмулятор банковских сервисов. Удобство запуска всех сервисов одной командой упрощает процесс разработки и тестирования.
Selenide – библиотека, которая обеспечивает простоту использования для тестирования веб-приложений, гарантируя стабильность и надежность при работе с динамическими элементами страницы.
WebDriver – стандартный инструмент для управления браузерами, который отлично работает в сочетании с Selenide.
JUnit – мощный фреймворк для написания и организации тестов, поддерживающий аннотации, параметризацию и гибкую настройку тестов.
Allure – инструмент для создания визуально привлекательных и подробных отчетов о результатах тестирования, что позволяет лучше анализировать выполненные тесты.
Библиотека Faker – удобный инструмент для генерации тестовых данных, что значительно упрощает процесс разработки тестовых сценариев.
Библиотека Lombok – помогает уменьшить объем шаблонного кода в Java-приложениях, автоматизируя создание геттеров, сеттеров, конструкторов и других стандартных методов, что делает код более читаемым и легким для поддержки.
Перечень и описание возможных рисков при автоматизации:
Непредсказуемое поведение эмулятора банковских сервисов: некорректная работа эмулятора может привести к ложным результатам тестирования.
Временные задержки в ответах сервисов: задержки могут вызвать нестабильность и непредсказуемость результатов тестов.
Динамическое поведение элементов: задержки в загрузке некоторых элементов могут негативно повлиять на стабильность тестов.
Проблемы с доступом: недоступность тестового сервера или базы данных может остановить процесс тестирования.
Некорректные данные: использование неправильных тестовых данных может вызвать ошибки в тестах.
Отсутствие интернет-соединения: недостаток подключения к интернету может замедлить процесс тестирования.
Интервальная оценка с учетом рисков в часах:
Исследование и анализ: 4-10 часов.
Настройка окружения (Docker, Docker Compose): 4-6 часов.
Разработка тестовых сценариев: 5-12 часов.
Написание автотестов: 20-30 часов.
Тестирование и отладка: 16-24 часа.
Подготовка отчётных документов по итогам автоматизированного тестирования: 4 часа.
Подготовка отчётных документов по итогам автоматизации: 4 часа.
Итого: 57-90 часов.

План сдачи работ:
Автотесты: будут готовы через 2 недели.
Результаты прогона автотестов: будут готовы через 2 недели и 5 дней.
Отчёт по автоматизации: будет загружен в репозиторий через 3 недели.