ODD-EVEN-GAME--HOMEWORK--10--WEEK-10
====================================

ODD-EVEN GAME HOMEWORK #10- WEEK 10


//  BY REINA OLARTE

//   HOMEWORK #10 WEEK 10

import java.util.Scanner;

public class OddEvenGame 
{
	public static void main(String[] args)
	{
		int lowint;
		int highint;
		boolean SIGA = true;

		Scanner input = new Scanner(System.in);

		//  new object OddEven
		//  constructor
		while(	SIGA)
		{

		System.out.println("Hi!!!LETS GO TO PLAY ; pLease input a low integer:");
		lowint = input.nextInt();
		System.out.println("Please input a high integer:");
		highint = input.nextInt();

		OddEven myGame = new OddEven(lowint, highint);
		//Display welcome message
		myGame.displayMessage();
		//Start the Game
		myGame.playGame();
		//Display results
		myGame.displayResults();
		SIGA = myGame.keepPlaying();
		//myGame.GetKeepPlaying();
		}	
	}
}
