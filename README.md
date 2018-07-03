# Lesson1HT1
TODO: 02.07.2018 Реализовать функции для подсчета числа в указанной степени, извлечение квадратного корня из числа

package com.company;
import java.util.Scanner;
public class Main {

    public static void main(String[] args) {
        int a;
        int b;
        int c;
        Scanner in = new Scanner(System.in);
        System.out.println("Введите целое число");
        a = in.nextInt();
        System.out.println("Введите степень");
        b = in.nextInt();
        System.out.println("Результат:" + Math.pow(a, b));
    }
}
