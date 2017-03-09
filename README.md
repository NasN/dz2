package com.company;

import java.lang.String;
import java.util.Arrays;
import java.util.Scanner;

public class Main {

    public static void main(String[] args) {
        {
            System.out.print("Циклы 1 задание:" + Arrays.deepToString(matrixA(3, 3)) + "\n");
            System.out.println();
        }
        {
            System.out.print("Введите значение(Логические выражения 1 задание):");
            System.out.print(cigarParty(40, true)+ "\n");
        }
        {
            System.out.print("Введите i(Логические выражения 2 задание):");
            System.out.println(dateFashion(8,10));
        }
        {
            System.out.print("Введите значение(Логические выражения 3 задание):");
            System.out.print(squirrelPlay(40, true) + "\n");
        }
    }
    public static int[][] matrixA(int i, int j) {
        int[][] matrixA;
        matrixA = new int[3][3];
        matrixA[0][0] = 1;
        matrixA[0][1] = 0;
        matrixA[0][2] = 0;
        matrixA[1][0] = 0;
        matrixA[1][1] = 1;
        matrixA[1][2] = 0;
        matrixA[2][0] = 0;
        matrixA[2][1] = 0;
        matrixA[2][2] = 1;
        for (i = 0; i < 3; i++) {
            if (i > 3) {
                break;
            }
            for (j = 0; j < 3; j++) {
                if (j > 3) {
                    break;
                }
            }
        }
        return matrixA;
    }

    public static boolean cigarParty (int b, boolean a) {
        Scanner num = new Scanner(System.in);
        b = num.nextInt();
        if (b >= 30 && b <= 60) {
            return true;
        } else if (b >= 60) {
            return true;
        } else if (b <= 30) {
            return false;
        }
        return true;
    }

    public static int dateFashion (int i, int j){
        Scanner num = new Scanner(System.in);
        if (i >= 8) {
            return 2;
        }else if (i <= 2) {
            return 0;
        }else if (i >=3 || i <= 7) {
            return 1;
        }
        if (j >= 8) {
            return 2;
        }else if (j <= 2) {
            return 0;
        }else if (j >=3 || j <= 7) {
            return 1;
        }
        return 1;
    }

    public static boolean squirrelPlay(int i, boolean inSummer) {
        Scanner num = new Scanner(System.in);
        i = num.nextInt();
        if (inSummer == true && i >= 20 && i <= 30) {
            return true;
        } else if (inSummer == true && i >= 31 && i <= 50) {
            return true;
        }
        return false;
    }
}
