# Assignment1
import java.util.Scanner;
class JAVA
{
    public static void main(String[] args)
{
        Scanner scanner = new Scanner(System.in);
        int rows = 2;
        int column = 3;
        int[][] matrix = new int[rows][column];
        
        System.out.println("Enter elements for a 2x3 matrix:");
        for (int i = 0; i < rows; i++) {
            for (int j = 0; j < column; j++) {
                System.out.print("Element [" + i + "][" + j + "]: ");
                matrix[i][j] = scanner.nextInt();
            }
        }
        
        System.out.println("Given matrix is:");
        for (int i = 0; i < rows; i++) {
            for (int j = 0; j < column; j++) {
                System.out.print(matrix[i][j] + "\t");
            }
            System.out.println();
        }
        
        int sum = 0;
        for (int i = 0; i < rows; i++) {
            for (int j = 0; j < column; j++) {
                sum= sum + matrix[i][j];
            }
        }
        System.out.println("Sum of Matrix: " + sum);
    }
}
