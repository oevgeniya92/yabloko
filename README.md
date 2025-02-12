# yabloko

public class FactorialCalculator {
    public static void main(String[] args) {
        int number = 5; // Можно изменить число для других расчетов

        long factorialResult = calculateFactorial(number);
        System.out.printf("Факториал числа %d равен %d%n", number, factorialResult);
    }

    public static long calculateFactorial(int n) {
        if (n == 0 || n == 1) {
            return 1;
        }

        long result = 1;
        for (int i = 2; i <= n; i++) {
            result *= i;
        }
        return result;
    }
}
