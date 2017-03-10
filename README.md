package com.company;

import java.lang.String;
import java.util.Arrays;

public class Main {

    public static void main(String[] args) {
        {
            System.out.print("Циклы 1 задание:" + Arrays.deepToString(matrixA(3, 3)) + "\n");
            System.out.println();
        }
        {
            System.out.print("cigarParty(Логические выражения 1 задание):");
            System.out.print(cigarParty(40, true) + "\n");
        }
        {
            System.out.print("dateFashion(Логические выражения 2 задание):");
            System.out.println(dateFashion(8, 10));
        }
        {
            System.out.print("squirrelPlay(Логические выражения 3 задание):");
            System.out.print(squirrelPlay(40, true) + "\n");
        }
        {
            System.out.print("caughtSpeeding(Логические выражения 4 задание):");
            System.out.print(caughtSpeeding(50, true) + "\n");
        }
        {
            System.out.print("sortaSum(Логические выражения 5 задание):");
            System.out.print(sortaSum(10, 4) + "\n");
        }
        {
            System.out.print("love6(Логические выражения 6 задание):");
            System.out.print(love6(6, 4) + "\n");
        }
        {
            System.out.print("love6(Логические выражения 7 задание):");
            System.out.print(in1To10(7, true) + "\n");
        }
        {
            System.out.print("answerCell(Логические выражения 8 задание):");
            System.out.print(answerCell(false, false, true) + "\n");
        }
        {
            System.out.print("noTeenSum(Логические выражения 9 задание):");
            System.out.print(noTeenSum(2, 1, 14) + "\n");
        }
//        {
//            System.out.print("blackjack(Логические выражения 10 задание):");
//            System.out.print(blackjack(19,21)+ "\n");
//        }
        {
            System.out.print("loneSum(Логические выражения 11 задание):");
            System.out.print(loneSum(3, 3, 3) + "\n");
        }
        {
            System.out.print("luckySum(Логические выражения 12 задание):");
            System.out.print(luckySum(1, 13, 3) + "\n");
        }
        {
            System.out.print("evenlySpaced(Логические выражения 13 задание):");
            System.out.print(evenlySpaced(4,6,2) + "\n");
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
    public static boolean cigarParty(int b, boolean a) {
        if (b >= 30 && b <= 60) {
            return true;
        } else if (b >= 60) {
            return true;
        } else if (b <= 30) {
            return false;
        }
        return true;
    }
    public static int dateFashion(int i, int j) {
        if (i >= 8) {
            return 2;
        } else if (i <= 2) {
            return 0;
        } else if (i >= 3 || i <= 7) {
            return 1;
        }
        if (j >= 8) {
            return 2;
        } else if (j <= 2) {
            return 0;
        } else if (j >= 3 || j <= 7) {
            return 1;
        }
        return 1;
    }
    public static boolean squirrelPlay(int i, boolean inSummer) {
        if (inSummer == true && i >= 20 && i <= 30) {
            return true;
        } else if (inSummer == true && i >= 31 && i <= 50) {
            return true;
        } else if (inSummer == false && i >= 51) {
            return false;
        }
        return false;
    }
    public static int caughtSpeeding(int speed, boolean a) {
        if (speed <= 60) {
            return 0;
        } else if (speed >= 61 && speed <= 80) {
            return 1;
        } else if (speed >= 81) {
            return 2;
        }
        return 2;
    }
    public static int sortaSum(int a, int b) {
        int sum;
        sum = a + b;
        if (sum >= 10 && sum <= 20) {
            return a + b;
        }
        return 20;
    }
    public static boolean love6(int a, int b) {
        int sum, raznost;
        sum = a + b;
        raznost = a - b;
        if (sum == 6 || raznost == 6) {
            return true;
        } else if (a == 6 || b == 6) {
            return true;
        }
        return true;
    }
    public static boolean in1To10(int n, boolean a) {
        if (n >= 1 && n <= 10) {
            return true;
        } else if (n <= 1 && n >= 10) {
            return true;
        }
        return false;
    }
    public static boolean answerCell(boolean isMorning, boolean isMom, boolean isSleeping) {
        if (isMorning == true && isMom == false) {
            return false;
        } else if (isSleeping == true) {
            return false;
        }
        return true;
    }
    public static int noTeenSum(int a, int b, int c) {
        if (a >= 13 && a <= 14) {
            a = 0;
        } else if (a >= 17 && a <= 19) {
            a = 0;
        } else if (b >= 13 && b <= 14) {
            b = 0;
        } else if (b >= 17 && b <= 19) {
            b = 0;
        } else if (c >= 13 && c <= 14) {
            c = 0;
        } else if (c >= 17 && c <= 19) {
            c = 0;
        }
        return a + b + c;
    }
    //    public static int blackjack(int a, int b) {
//        if (a >= 0 && b <= 21) {
//            return a;
//        } else if (a <= 0 && b >= 21) {
//            return b;
//        }
//        return a;
////        if (b >= 0 && b <= 21) {
////            return ;
////        } else if (b <= 0 && b >= 21) {
////            return 0;
////        }
////        return 0;
//    }
//}
    public static int loneSum(int a, int b, int c) {
        if (a == b && a == c && b == c) {
            return 0;
        } else if (a == b) {
            return c;
        } else if (a == c) {
            return b;
        } else if (b == c) {
            return a;
        }
        return a + b + c;
    }
    public static int luckySum(int a, int b, int c) {
        if (a >= 13) {
            return 0;
        } else if (b >= 13) {
            return a;
        } else if (c >= 13) {
            return a + b;
        }
        return a + b + c;
    }
    public static boolean evenlySpaced(int a, int b, int c) {
        if (a + b == c || b + c == a || a + c == b) {
            return true;
        }
        return false;
    }
}
