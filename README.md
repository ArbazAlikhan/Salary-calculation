//# Salary-calculation
//C# Program for Salary calculation//


using System;
					
public class Program
{
	public static void Main()
	{
		int option;
        double  gsal;
        gsal=0;
        int Basic;
        double HRA;
        double DA;
        int TA;
        TA=2500;
        int Medi;
        Medi= 4000;
		
		Console.WriteLine("Enter Designation");
		Console.WriteLine("1.trainee\n 2.ProjeectManager\n 3. Team Lead");
        option=Convert.ToInt32(Console.ReadLine());
      switch(option)
      {
      case 1:
          Console.WriteLine("Basic Salary:");
          Basic=Convert.ToInt32(Console.ReadLine());
          HRA=0.6*Basic;
          DA= 0.3*Basic;
          gsal=Basic+HRA+DA+TA+Medi;
          break;
      case 2:
          Console.WriteLine("Basic Salary:");
          Basic=Convert.ToInt32(Console.ReadLine());
          HRA=0.7*Basic;
          DA= 0.4*Basic;
          gsal=Basic+HRA+DA+TA+Medi;
          break;
      case 3:
          Console.WriteLine("Basic Salary:");
          Basic=Convert.ToInt32(Console.ReadLine());
          HRA=0.8*Basic;
          DA= 0.5*Basic;
          gsal=Basic+HRA+DA+TA+Medi;
          break;
      default:
          Console.WriteLine("incorrect option selected");
		 break;

      }
      Console.WriteLine(" The gross Salary of the selected employee is :{0}",gsal);
      Console.ReadLine();

     }
  }
