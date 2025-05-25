# Антонио Цековски 161241

## Барање 2 - Control Flow Graph

![SI-lab2](https://github.com/user-attachments/assets/1c7ca0ab-1b84-4949-a998-d86b2bca5f83)

## Барање 3 - Цикломатска комплексност

Цикломатската комплексност на овој код е 9, истата ја добив преку формулата E-N+2C, каде E е бројот на ребра, N е бројот на темиња и C е бројот на поврзани компоненти, во нашиот случај E = 33, N = 26, C = 1, според тоа E-N+2*1 = E-N+2 = 33 - 26 + 2 = 9, исто така може да се добие и преку формулата P+1, каде што P е бројот на предикатни јазли. Во случајoв P = 8, па цикломатската комплексност изнесува 9.

## Барање 4 - Every Statement критериум

1. AllItems == null ,      Nodes : start, 1, 2, end
2. item.getName() == null  Nodes : start, 1, 3, 4, 5, 6, 7, 8, end
3. item.getDiscount() > 0  Nodes : start, 1, 3, 4, 5, 6, 7, 9, 11, 12, 14, 15, 16, 17, 18, 19, 20, 21, 22, end
4. item.getDiscount() <= 0 Nodes : start, 1, 3, 4, 5, 6, 7, 9, 11, 13, 15, 16, 17, 18, 19, 20, 21, 24, end 
5. cardnumber е невалиден  Nodes : start, 1, 3, 4, 5, 6, 7, 9, 11, 13, 14, 15, 23, end

Со овие тест случаи се постигнува Every Statement критериумот.

## Барање 5 - Multiple Condition критериум

if (item.getPrice() > 300 || item.getDiscount() > 0 || item.getQuantity() > 10)
1.          T                          X                        X
2.          F                          T                        X
3.          F                          F                        T
4.          F                          F                        F

Минимално се потребни овие 4 тест случаи.

