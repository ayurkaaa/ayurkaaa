using System;
class Program
{
    static void Main(string[] args)
    {
        Console.WriteLine();
        int n = int.Parse(Console.ReadLine());
        int[] array = new int[n];
        Random random = new Random();
        for (int i = 0; i < n; i++)
        {
            array[i] = random.Next(1, 70);
            Console.Write(array[i] + " ");
        }
        Console.WriteLine();
        for (int i = 0; i < array.Length; i++)
        {
            int b = random.Next(array.Length);
        int new1 = array[i];
            array[i] = array[b];
            array[b] = new1;
        }
        for (int i = 0; i < array.Length; i++)
        {
            Console.Write(array[i] + " ");
        }
    }
}
