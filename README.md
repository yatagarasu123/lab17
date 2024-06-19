### Лабораторна робота №17: Generators and Data structures

#### Мета роботи:
Ознайомлення з генераторами в Python та робота зі структурами даних.

#### Опис завдання:
В даній лабораторній роботі реалізовані генератори для ітерації та обробки різних типів даних: списків, файлів, дерев, матриць та інших.

#### Виконання роботи:
Структура проекту:
Кожен генератор відповідає за окреме завдання з відповідною назвою.

#### Опис файлів:
- `generators.py`: містить реалізації всіх генераторів.
- `README.md`: описує структуру проекту, основні функції та приклади їх використання.

#### Опис основних функцій та методів з поясненням їх роботи:

**Task 1: number_generator(numbers)**  
Генерує числа зі списку по одному.

```python
def number_generator(numbers):
    for num in numbers:
        yield num
```

Приклад використання:
```python
gen = number_generator([1, 2, 3, 4, 5])
print(next(gen)) 
print(next(gen))
```

**Task 2: even_number_generator(start, end)**  
Генерує парні числа в заданому діапазоні.

```python
def even_number_generator(start, end):
    for num in range(start, end + 1):
        if num % 2 == 0:
            yield num
```

Приклад використання:
```python
gen = even_number_generator(1, 10)
print(next(gen))  
print(next(gen))  
```

**Task 3: odd_number_generator(start, end)**  
Генерує непарні числа в заданому діапазоні.

```python
def odd_number_generator(start, end):
    for num in range(start, end + 1):
        if num % 2 != 0:
            yield num
```

Приклад використання:
```python
gen = odd_number_generator(1, 10)
print(next(gen))  
print(next(gen)) 
```

#### Результати:
Кожен генератор виконує вказану функцію, повертаючи значення по одному.
![image](https://github.com/yatagarasu123/lab17/assets/145234911/9b44b48d-0440-4796-ba23-5e5da742ad0e)
![image](https://github.com/yatagarasu123/lab17/assets/145234911/3336a78d-ed83-4a22-911b-943054b2a03d)
![image](https://github.com/yatagarasu123/lab17/assets/145234911/8c97f5b9-f94e-4bba-a33e-5f15d8b892a4)


#### Висновки:
Лабораторна робота дозволила розібратися з особливостями роботи генераторів у Python та їх застосуванням для різних типів даних.

#### Інструкції з запуску:
Для використання генераторів необхідно викликати відповідні функції з необхідними аргументами та обробити результати.
