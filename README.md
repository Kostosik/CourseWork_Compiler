# Объявление вещественной константы с инициализацией на языке Java

## Примеры допустимых строк
```
final double PI = 3.141592653589793;
```

## Разработанная грамматика
```
<DEF> -> 'final' <FINAL>
<FINAL> -> 'double' <TYPE>
<TYPE> -> <IDENT>
<IDENT> -> LETTER (DIGIT | LETTER | '_')* <EQUALS>
<EQUALS> -> '=' <NUMBER>
<NUMBER> -> DIGIT+ <POINT> + <NUMAFTERPOINT> 
<NUMAFTERPOINT> -> DIGIT +<SEMICOLON>
<SEMICOLON> -> ';' <END>
```

## Граф конечного автомата
![alt text](graph.png)

## Тестовые примеры
![alt text](image-6.png)
![alt text](image-7.png)
