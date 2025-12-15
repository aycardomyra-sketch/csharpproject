using System;

namespace MyProject
{
	public class task2
	{
		public static void Main (string[] args)
		{
			//Declare and initialize the 2D array
			int [][] numberMatrix =new int[][]
			{
				new int [] {2,4,6,8,10}, //Row 0:Even numbers 
				new int [] {1,3,5,7,9} //Row 1:Odd numbers 
			};
			Console.WriteLine("The number matrix has been initialized.");
			
			//Extract the digits based on the puzzle clues
			int digit1=numberMatrix [1] [3]; //Row1, Index3
			int digit2=numberMatrix [0] [0]; //Row0, Index0
			int digit3=numberMatrix [1] [4]; //Row1, Index4
			
			//Combine the digits into a single string (3-digit key)
			string key =$"{digit1}{digit2}{digit3}";
			
			//display the password 
			Console.Write($"The 3-digit password is: {key}");
		}
	}
}
