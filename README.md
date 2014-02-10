Random
======

The program which will help you to count faster. 


Enter the program, choose the difficulty level by pressing 1, 2, 3, 4, 5, 6, 7. 
Then bigger number then longer variables thet you will have to count.
Program creates 6 variables of your chosen difficulty. 


Afterwards it asks you about quantity of variables you would like to count and depending on your ansver (from 1 to 6) 
chooses the formula and prints the result.

Then it asks you to input your own result and, if it was not right, givs one more chance to answer this time correctly.
For the correct answer from the first time you will see '='+ result + 'perfect' on your screen.
For the correct answer from the second time ('Lasr chance') it won`t be written any 'perfect'. Just '=' + result.


Example:
Program: Choose the difficulty level by pressing 1, 2, 3, 4, 5, 6 or 7 number button. Then bigger number, then more difficult level you get.'
Me: 3

Program: How many variables would you like to use? Enter the number of them.
Me: 4

Text on the screen: 456 + 678 + 123 + 890

Program: Result?
Me: 7890

Program: Last chance.
Me: 2147

Text on the screen: = 2147

<html>
<head>
<script type='text/javascript'>
//Программа для тренировки счёта, позволяющая выбирать количество
//переменных и их разрядность.
function start() {//Функция, определяющая программу. Запускается при загрузке страницы.
var m, varn, n, t, f, th, s, fi, se, te, cont;//Объявление переменных.
n = prompt('Choose the difficulty level by pressing 1, 2, 3, 4, 5, 6 or 7 number button. Then bigger number, then more difficult level you get.', '');
switch(n){
    case '1':
    {var m = 100;//Количество нолей определяет 
     break};     //длину (разрядность) числа = m.
    case '2':
    {var m = 1000;
     break;}
    case '3':
    {var m = 10000;
     break;}
    case '4':
    {var m = 100000;
    break;}
    case '5':
    {var m = 1000000;
     break;}
    case '6':
    {var m = 10000000;
     break;}  
    case '7':
    {var m = 100000000;
     break;}
    default:
    {var m = 100;
    break}
}
f = Math.round(Math.random()* m); //Создание случайного числа (переменной)
th = Math.round(Math.random()* m); //и последующее его преобразование
s = Math.round(Math.random()* m);  //путём умножения на m.
fi = Math.round(Math.random()* m);
se = Math.round(Math.random()* m);
te = Math.round(Math.random()* m);
 
varn = prompt('How many variables would you like to use? Enter the number of them.','');
switch(varn){//Определение используемой формулы, количества переменных и выводимого текста.
    case '2':
    {var t = f+s;//Используемая формула и количество переменных.
     document.write(f, '+', s);//Выводимый текст.
     break;
    };
    case '3':
    {var t = f+s+th;
     document.write(f, '+', s, '+', th);
     break;
    };
    case '4':
    {var t = f+s+th+fi;
     document.write(f, '+', s, '+', th, '+', fi);
     break;
    };
    case '5':
    {var t = f+s+th+fi+se;
     document.write(f, '+', s, '+', th, '+', fi, '+', se);
     break;
    };
    case '6':
    {var t = f+s+th+fi+se+te;
     document.write(f, '+', s, '+', th, '+', fi, '+', se, '+', te);
     break;
    };
    default:
    {var t = f+s;
     document.write(f, '+', s);
     break;
    }; 
}
var sum=prompt('Result?', '');//Запрос суммы.
 if(true){setTimeout(perf, 3000)//Правильное решение, функция perf.
    if (sum==t){document.write('='+t+' '+'perfect')}//Правильное решение, функция perf. 
//Выполняет те же функции, что и предыдущая строка, но по 
//отдельности они не работают.
    else{alert('try again');prompt('Last chance.', '')}//Дополнительный запрос решения, в случае неправильного ответа, его отсутствия или невалидности.
               if(true){(unperf)//Запуск функции правильного ответа.
               if (sum==t){perf}//Запуск функции неправильного ответа.
               else{document.write('='+t)}};};
function perf(){document.write('='+t+' '+'perfect')}//Печать решения + perfect (похвала).
 
function unperf(){
document.write('='+t)}//Печать решения.
 }
</script>
</head>
<body onload='start()'>
</body>
</html>
 







 
 

