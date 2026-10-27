import java.util.*;

class MainAPP37 {
    public static void main(String[] args)
 {
        Scanner sc = new Scanner(System.in);

        try 
{
            System.out.print("Enter size of array: ");
            int n = sc.nextInt();

            int[] arr = new int[n];

            for (int i = 0; i < n; i++) {
            System.out.println("Enter the element value:");
            arr[i] = sc.nextInt();
}

            System.out.println("Enter the index to fetch the value:");
            int index = sc.nextInt();

            System.out.println("Value at index " + index + " is: " + arr[index]);
}
            catch (ArrayIndexOutOfBoundsException e)
{
            System.out.println("Invalid index position entered");
}
            catch (InputMismatchException e)
{
            System.out.println("Error occurred");
}

            System.out.println("End of code");

            sc.close();
}
}

