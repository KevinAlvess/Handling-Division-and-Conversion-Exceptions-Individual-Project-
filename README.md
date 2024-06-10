# Handling-Division-and-Conversion-Exceptions-Individual-Project-
{
    class Program
{
    Static void Main(string[] args)
    int number;
    {
       Console.Writeline("Hello please enter two numbers to be divided.")

        Console.Writeline("Enter the first number: ");
        string input1 = Console.Readline();

        Console.Writeline("Enter the second number:");
        string input2 = Console.Readline();

        try
    {
        int number1 = Convert.ToInt32(input1);
        
        int number2 = Convert.ToInt32(input2);

        int result = Divide(number1, number2);
        Console.Writeline($"The answer provided was invalid {number1} when divided by {number2} is: {result}");
    }
    catch(FormatException ex)
    {
        Console.WriteLine("There was an Error: There may be one or more input that are not valid integers.");
        Console.WriteLine($"Detailed error message: {ex.Message}");
    }
    catch (DivideByZeroException ex)
    {
        Console.WriteLine("There was an Error: Division by zero is not allowed.");
    }
    catch (OverFlowException) {
        Console.WriteLine("There was an Error caught: {Number1}", number2);
        Console.WriteLine($"Detailed error message: {ex.Message}");
    }

    catch (OverFlowException) {
        Console.WriteLine("There was an Error caught: {Number12", number1);
        Console.WriteLine($"Detailed error message: {ex.Message}");
    }
    {
    Console.WriteLine("You may press any key to exit the program.");
    console.ReadKey();
    }
    
        static int Divide(int a, int b)
    {
    return a / b;
}
