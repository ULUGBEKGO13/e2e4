# using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Collections;
					
public class Program
{
	public static void Main(double n)
	{
		int a = 0;
		n = 1;
		int k = 0;
		ArrayList list = new ArrayList();
		for (int i1 = 1; i1 < 53; ++i1)
		{
			for (int i2 = 1; i2 < 53; ++i2)
			{
				for (int i3 = 1; i3 < 53; ++i3)
				{
					list.Add(i1+""+i2+""+i3);
					k++;
					if((i1 == 3) && (i2 == 7) && (i3 == 12))
					{
						a = k;
					}
				}
			}
		}
		Console.WriteLine(a);
		while(n<((factor(52)*factor(52))*2))
		{
			
		}
	}
	static double factor(double n)
	{
		double r = 1;
		for(double i = r + 1; i<n; i++)
		{
			r = r*i;
		}
		return r;
	}
}
