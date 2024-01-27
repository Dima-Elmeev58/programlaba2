# programlaba2
package com.company;
import java.util.Scanner;
public class Main {

    public static void main(String[] args) {
        // write your code here
        Scanner input = new Scanner(System.in);
        System.out.println("Введите D");
        double D = input.nextDouble();
        double result = 0;
        System.out.println("Введите x");
        double x = input.nextDouble();
        System.out.println("Введите n");
        double n = input.nextDouble();
        if (x > -1 && x <= 1){
            for(int i = 0; i <= D; i++){
                double b = (Math.pow(-1, n) * Math.pow(x, n + 1)) /n + 1;
                result += b;
            }
            System.out.println(result);
        }
        else{
            System.out.print("Ошибка, x должен принадлеать промежутку (-1; 1)");
        }
    }
    }
