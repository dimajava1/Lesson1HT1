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

TODO: 02.07.2018 Дополнительно - реализовать решение квадратного уравнения через функцию(добавить дополнительный параметр)

package com.company;
import java.util.Scanner;

public class Main {

    public static void main(String[] args) {
        double a, b, c;
        double Diskremenant;
// на всякий случай использую double
        System.out.println("Программа решает квадратное уравнение вида:");
        System.out.println("ax^2 + bx + c = 0");
        System.out.println("Введите a, b и c  (в новой строке кажое число):");
        Scanner in = new Scanner(System.in);
        a = in.nextDouble();
        b = in.nextDouble();
        c = in.nextDouble();
        Diskremenant = b * b - 4 * a * c;
        //формула дискрименанта
        //условный оператор "ести.., то.., в другом случае..."
        if (Diskremenant > 0) {
            double x1, x2;
            x1 = (-b - Math.sqrt(Diskremenant)) / (2 * a);
            x2 = (-b + Math.sqrt(Diskremenant)) / (2 * a);
            System.out.println("Корни уравнения: x1 = " + x1 + ", x2 = " + x2);
        } else if (Diskremenant == 0) {
            double x;
            x = -b / (2 * a);
            System.out.println("Уравнение имеет единственный корень: x = " + x);
        } else {
            System.out.println("Уравнение не имеет решения!");
        }
    }
}
