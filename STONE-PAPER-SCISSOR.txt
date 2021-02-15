import java.util.Scanner;
import java.util.Random;
public class AddTwoIntegers
{
	public static void main (String args [])
	{
		Scanner M = new Scanner (System.in);
		Random  R = new Random();
		int Z = 0;
		int V = 0;
		int Y = 0;
		
		System.out.println("enter the 0 = Rock , 1 = paper, 2 = scissor");
		
		for(int i=0; i<3;i++ )
		{
			int o = M.nextInt();
			int t = R.nextInt(3);
			
		System.out.println("user input is " +o+ " Computer respons "+t);
		
		 if(o==1&&t==2||o==0&&t==1||o==2||t==0)
		 {
			 V++;
			 System.out.println("you lose this round");
		 }
		 else if (o==2&&t==2||o==1&&t==1||o==0&&t==0)
		 {
			 System.out.println("oooho ... you and computer are same");
			 Y++;
			
		 }
		 else if (o==0&&t==2|| o==1&&t==0 || o==2&&t==1 )
		 {
			 Z++;
			 System.out.println("yee.. you won this round");
		 }
		 
		 
		}
		
	switch(Z)
	{
	case 2:
		System.out.println("**YEaah you won this round**");
		break;
	case 3:
		System.out.println("**YEaah you won this round**");
		break;
	}
	
	switch(V)
	{
	case 2:
		System.out.println("## oohno officialy you lose this game ##");
		break;
	case 3:
		System.out.println("## ohhno.. officialy you lose this round ##");
		break;
	}
	
	switch(Y)
	{
	case 2:
		System.out.println(" hold on you and computer is same");
		break;
	case 3:
		System.out.println("Hold on you and computer is same");
	}
	}
}
