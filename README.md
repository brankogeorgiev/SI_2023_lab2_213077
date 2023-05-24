# Втора лабораториска вежба по предметот Софтверско Инженерство
## Бранко Георгиев, 213077

### Control Flow Graph
![cfg](https://github.com/brankogeorgiev/SI_2023_lab2_213077/assets/75042838/b5d60558-b9b5-4e49-a30b-5df01db3464a)


### Цикломатска комплексност
Цикломатската комплексност на овој код е 11 и истата ја добив на 2 начини:

    1. Број на ребра - број на јазли + 2 (31 - 22 + 2 = 11)
    
    2. Број на региони + 1 (10 + 1 = 11)
    
### Тест случаи според критериумот Every Branch
    1. user = null, allUsers = X
    2. user.username = null, user.pass = "12345", user.email = "email@gmail.com", allUsers = [diff, diff, same]
    3. user.username = "username", user.email = "none",  user.pass = "123456789", allUsers = [X]
    4. user.password = "123 654321", allUsers = []
    5. user.password = "1234567#!", user.email = "none", user.username = "username", allUsers = []


### Тест случаи според критериумот Multiple Condition
    1. User = null
    2. User != null, user.password = null
    3. User != null, user.password != null, user.email = null
    4. User != null, user.password != null, user.email != null


#### Опис на кратенките
    X = Било што
    diff = се работи за user со различни лични информации (различен корисник)
    same = се работи за user со исти лични информации (ист корисник)
