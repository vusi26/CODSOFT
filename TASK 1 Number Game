package number.guessing.game;
import java.util.Scanner;

public class NumberGuessingGame {

   
    public static void main(String[] args) {
      Scanner input = new Scanner(System.in);
     System.out.println ("Generate a random number between 1 and 100.");
     
     boolean playAgain= true;
     int TotalAttempts=0;
     int roundsWon=0;
     
     while(playAgain) {
     int number = (int)(Math.random()*100)+ 1;
    
     int NumberGuessing;
     int attempts=0;
     boolean guessedCorrectly=false;
     final int maxAttempts = 5;//limiting the number of attempts to five
     
     while(!guessedCorrectly && attempts < maxAttempts) {
      System.out.print("\nEnter your guess:");
      NumberGuessing=input.nextInt();
      attempts++;
      TotalAttempts++;
      
      if (NumberGuessing ==number){
      System.out.println("Congratulations!You've guessed the number" + number + "correctly.");
      System.out.println("it took you" + attempts + "attempts to guess the number.");
      guessedCorrectly = true;
      roundsWon++;
      }else if (NumberGuessing < number) {
       System.out.println("Your guess is too low. Try again.");
      }else {
       System.out.println("Your guess is too high. Try again");
          
      }
      
      } 
    
        System.out.println("\nDo you want to play again?(yes/no): ");
        String playChoice =input.next().toLowerCase();
        if(!playChoice.equals("yes")) {
            playAgain = false;
        }
        
     }
         System.out.println("\nGame Over!");
         System.out.println("You played" + (TotalAttempts /5)+ "rounds.");
         System.out.println("You won"+  roundsWon + "rounds.");
         input.close();
    }
}
