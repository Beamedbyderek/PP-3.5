package pp.pkg3.pkg5;

/*

10/13/2022

Derek Durand

generates phone number

*/
   import java.util.Scanner;  
public class PP35 {



public static void main(String[] args) {
    Scanner input = new Scanner(System.in);
    System.out.println("Enter a coordinate: ");
    String coordinate = input.nextLine();
    String[] parts = coordinate.split(",");
    String x = parts[0];
    String y = parts[1];
    
    System.out.println("Enter another coordinate: ");
    String coordinate2 = input.nextLine();
    String[] parts2 = coordinate2.split(",");
    String x2 = parts2[0];
    String y2 = parts2[1];
    
    double x3 = Double.parseDouble(x); 
    double y3 = Double.parseDouble(y);
    double x4 = Double.parseDouble(x2);
    double y4 = Double.parseDouble(y2);
    System.out.println("x: " + x3 + "\ny: " + y3);
    System.out.println("x: " + x4 + "\ny: " + y4);
    double result = Math.sqrt(((x4 -x3)*(x4 - x3)+(y4 - y3)*(y4 - y3)));
    System.out.println(String.valueOf(result));
}
}
