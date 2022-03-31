# Write-a-program-that-allows-the-user-to-enter-a-student-number-Then-check-if-the-code-is-correct-in-
The student ID format is “Bxxxxxxx” where x is an integer from 1-9. (Use a regular expression to bind the format)
import java.util.Scanner;

public class BaiTapJavaCoBan5 {
    public static void main(String[] args)
    {
       String MSSV;
       System.out.println("Enter MSSV:");
       Scanner sc = new Scanner(System.in);

       MSSV = sc.nextLine(); // Get a string from the keyboard

       if (MSSV.matches("B\\d{7}")) //Check with regular expression
          System.out.println("Suitable");
       else
          System.out.println("Not suitable");

       // This article is advanced because it uses regular expressions
       // you can google to know more about it
    }
}
