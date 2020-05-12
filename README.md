import static java.lang.System.in;
import statci java.lang.System.out;
import java.util.Scanner;
import java.util.Random;

public class GuessingGame {
    public static void main(String[] args){
        
        Scanner keyboard = new Scanner(in);
        out.println("Enter a value from 1 to 20: ");
        
        int inputNumber = keyboard.next();
        int randomNumber = new Random(). nextInt(20) + 1;
        
        if (inputNumber == randomNumber)
        {
            out.println("************");
            out.println("*YOU WIN*");
            out.println("************");
        }
        
        else if (inputNumber > randomNumber)
        {
            out.print(inputNumber + " is greater than ");
            out.println("the range specified.");
            out.println("Please try again...");
        }
        
        else 
        {
            out.println("*SORRY YOU LOST*");
            out.print("The random number was: ");
            out.println(randonNumber + ".");
        }
        out.println("Thanks for playing.");
    }
}
