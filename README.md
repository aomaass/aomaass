from random import randint

def convertNumberToAction( number ):
    if number == 1:
        return 'Hammer'
    elif number == 2:
        return 'Paper'
    elif number == 3:
        return 'Scissors'  

def game():
    try:
        print('1 = '+convertNumberToAction(1))
        print('2 = '+convertNumberToAction(2))
        print('3 = '+convertNumberToAction(3))
        i = int(input('Please input number : '))
    except:
        i = 0

    if i > 0 :
        result = ''
        r = randint( 1, 3 )
        print('Computer '+convertNumberToAction(r)+' / You '+convertNumberToAction(i))
        if r == i :
            result = 'always'
        elif r == 1 and i == 2 :
            result = 'You Win'
        elif r == 2 and i == 1 :
            result = 'Computer Win'
        elif r == 2 and i == 3 :
            result = 'You Win'
        elif r == 3 and i == 2 :
            result = 'Computer Win'          
        elif r == 1 and i == 3 :
            result = 'Computer Win'      
        elif r == 3 and i == 1 :
            result = 'You Win'  

        print( result )                                     

game()- 👋 Hi, I’m @aomaass
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
aomaass/aomaass is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
