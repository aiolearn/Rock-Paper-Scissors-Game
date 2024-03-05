<h1 align="center">Welcome to Rock Paper Scissors Game 👋</h1>

# Rock Paper Scissors Game

In this project, we are going to make a rock-paper-scissors game using Python language and random module.

## Modules

In the module section, we use the random module so that the computer chooses between rock, paper and scissors randomly and is in front of our choice. In the second part, the computer code chooses one of the following three options

```Python
import random
bazi = ['sang', 'kaqaz', 'qeychi']
```

## Usage
In the first part, we set the computer variable to select the computer, and then we set the points for both teams to zero. And to start the game, we place correct and incorrect bets
```python
computer = ''
you_point = 0
computer_point = 0
shart_bazi = True
```

Here we have placed the conditions for the match, which are given below each condition.

```python
while(shart_bazi):
    you = input("Entekhab kon (sang, kaqaz, qeychi): ")

    # If the player enters '0', the game ends
    if you == "0":
        shart_bazi = False

    # Generate a random number to choose a computer move
    rand = random.randint(0, 2)
    computer = bazi[rand]

    # Checking the result of the game based on the choice of the player and the computer
    if you == 'sang' and computer == 'kaqaz':
        computer_point += 1

    if you == 'qeychi' and computer == 'kaqaz':
        you_point += 1

    if you == 'sang' and computer == 'qeychi':
        you_point += 1

    if you == 'kaqaz' and computer == 'qeychi':
        computer_point += 1

    if you == 'qeychi' and computer == 'sang':
        computer_point += 1

    if you == 'kaqaz' and computer == 'sang':
        you_point += 1

    # Display current scores and choices made
    print("YOU: (", you_point, ")", you, "     COM:(", computer_point, ")", computer)

    # The end of the game if the player or the computer reaches 3 points
    if you_point >= 3 or computer_point >= 3:
        shart_bazi = False
```
Determining the winner and displaying the scores
```python
if you_point > computer_point:
    print("\nYOU WIN!")
else:
    print("\nYOU LOSE :(")

print("YOU: ", you_point)
print("COM: ", computer_point)
```

## Result

This project was written by Majid Tajanjari and the Aiolearn team, and we need your support!❤️

# بازی سنگ کاغذ قیچی

در این پروژه قصد داریم با استفاده از زبان پایتون و ماژول رندوم یک بازی سنگ-کاغذ-قیچی بسازیم.

## ماژول ها

در قسمت ماژول از ماژول تصادفی استفاده می کنیم تا کامپیوتر بین سنگ، کاغذ و قیچی به صورت تصادفی یکی را انتخاب کند و در مقابل انتخاب ما قرار گیرد. در قسمت دوم کد کامپیوتر یکی از سه گزینه زیر را انتخاب می کند

```Python
import random
bazi = ['sang', 'kaqaz', 'qeychi']
```

## نحوه استفاده
در قسمت اول متغیر کامپیوتر را برای انتخاب کامپیوتر قرار می دهیم و سپس امتیاز هر دو تیم را صفر می کنیم. و برای شروع بازی شرط بندی درست و نادرست می گذاریم
```python
computer = ''
you_point = 0
computer_point = 0
shart_bazi = True
```

در اینجا شرایط مسابقه را قرار داده ایم که در زیر هر شرط آورده شده است.

```python
while(shart_bazi):
    you = input("Entekhab kon (sang, kaqaz, qeychi): ")

    # اگر بازیکن "0" را وارد کند، بازی به پایان می رسد
    if you == "0":
        shart_bazi = False

    # یک عدد تصادفی برای انتخاب یک حرکت کامپیوتری ایجاد کنید
    rand = random.randint(0, 2)
    computer = bazi[rand]

    # بررسی نتیجه بازی بر اساس انتخاب بازیکن و کامپیوتر
    if you == 'sang' and computer == 'kaqaz':
        computer_point += 1

    if you == 'qeychi' and computer == 'kaqaz':
        you_point += 1

    if you == 'sang' and computer == 'qeychi':
        you_point += 1

    if you == 'kaqaz' and computer == 'qeychi':
        computer_point += 1

    if you == 'qeychi' and computer == 'sang':
        computer_point += 1

    if you == 'kaqaz' and computer == 'sang':
        you_point += 1

    # نمایش نمرات فعلی و انتخاب های انجام شده
    print("YOU: (", you_point, ")", you, "     COM:(", computer_point, ")", computer)

    # پایان بازی اگر بازیکن یا کامپیوتر به 3 امتیاز برسد
    if you_point >= 3 or computer_point >= 3:
        shart_bazi = False
```
تعیین برنده و نمایش امتیازات
```python
if you_point > computer_point:
    print("\nYOU WIN!")
else:
    print("\nYOU LOSE :(")

print("YOU: ", you_point)
print("COM: ", computer_point)
```

## Result

این پروژه توسط مجید تجن جاری و تیم Aiolearn نوشته شده است و ما به حمایت شما نیازمندیم!❤️