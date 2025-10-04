import java.io.BufferedReader;
import java.io.InputStreamReader;

public class NumberOperations {

    public static void main(String[] args) {
        BufferedReader reader = new BufferedReader(new InputStreamReader(System.in));

        int a = readIntFromUser(reader, "Введите первое число (a):");
        int b = readIntFromUser(reader, "Введите первое число (b):");

        printResults(a, b);

    }

    public static int readIntFromUser(BufferedReader reader, String prompt) {
        while (true) {
            try {
                System.out.print(prompt);
                String input = reader.readLine();

                if (input == null || input.trim().isEmpty()) {
                    System.out.println("Ошибка! Вы не ввели число.");
                    continue;
                }

                int number = Integer.parseInt(input.trim());
                return number;

            } catch (Exception e) {
                System.out.println("Ошибка! Пожалуйста, вводите только целые числа.");
                System.out.println("Диапозон: от " + Integer.MIN_VALUE + " до " + Integer.MAX_VALUE);
            }
        }
    }


    private static void printResults ( int a, int b){

          // Сравнение чисел
          System.out.println("\nРезультаты сравнения");
          if (a > b) {
              System.out.println(a + " > " + b);
          } else if (a < b) {
              System.out.println(a + " < " + b);
          } else {
              System.out.println(a + " = " + b);
          }
  
          // Математические операции
          System.out.println("\nМатематические операции");
  
          // Сложение
          int sum = a + b;
          System.out.println(a + " + " + b + " = " + sum);
  
          // Вычитание
          int min = a - b;
          System.out.println(a + " - " + b + " = " + min);
  
          // Умножение
          int multi = a * b;
          System.out.println(a + " * " + b + " = " + multi);
  
          // Деление с проверкой деления на ноль
          if (b != 0) {
              double separation = (double) a / b;
              System.out.println(a + " / " + b + " = " + separation);
          } else {
                System.out.println(a + " / " + b + " = Ошибка! Деление на ноль невозможно.");
          }
        }
    }
