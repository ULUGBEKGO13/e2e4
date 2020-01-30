# 
static void Main(string[] args)
{
	double i1 = (factor(52) / (factor(52) * factor(1)));
        double i4 = (factor(12) / (factor(12) * factor(1)));
        double i3 = (52*52*2 + 52*6 + 12);
        Console.WriteLine(i3);
        Console.ReadKey();
}
static double factor(double n)
{
        double r = 1;
        for (double i = r + 1; i < n; i++)
        {
            r = r * i;
        }
        return r;
}
