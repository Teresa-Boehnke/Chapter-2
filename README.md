# Chapter-2
My codes for chapter 2

2.7

/**
 * Teresa Boehnke
 * 9/1/2o17
 * Convert
 * */
 import java.util.*; //Allows use of Scanner
 
 public class Convert
 {
     //Converts miles to kilometers
     
     public static void main (String[]args)
     {
         double miles, kilometers;
         
         miles = 6.7;
         kilometers = miles*1.60935;
         
         System.out.println ("Miles: " + miles);
         System.out.println ("Kilometers: " + kilometers);
         
     }//End main
 }//End class

2.8

/**
 * Teresa Boehnke
 * 9/1/2017
 * Distance
 * */
 import java.util.*; //Allows use of Scanner
 
 public class Distance
 {
     public static void main (String[]args)
     {
         int x1, x2, y1, y2;
         double distance;
         Scanner keyboard = new Scanner (System.in); //Creates an object for inputs
         
         System.out.print ("Enter x1: ");
         x1 = keyboard.nextInt();
         
         System.out.print ("Enter y1: ");
         y1 = keyboard.nextInt();
         
         System.out.print ("Enter x2: ");
         x2 = keyboard.nextInt();
         
         System.out.print ("Enter y2: ");
         y2 = keyboard.nextInt();
         
         distance = Math.sqrt(Math.pow ((x2 - x1), 2) + (Math.pow ((y2 - y1), 2)));
         
         System.out.println ("Coordinate 1: (" + x1 + ", " + y1 + ")");
         System.out.println ("Coordinate 2: (" + x2 + ", " + y2 + ")");
         System.out.println ("Distance: " + distance);
         
     }//End main
 }//End class

Extra

/**
 * Teresa Boehnke
 * 9/1/2017
 * Slope
 * */
 import java.util.*; //Allows use of Scanner
 
 public class Slope
 {
     public static void main (String[]args)
     {
         double x1, x2, y1, y2;
         double slope;
         Scanner keyboard = new Scanner (System.in); //Creates an object for inputs
         
         System.out.print ("Enter x1: ");
         x1 = keyboard.nextInt();
         
         System.out.print ("Enter y1: ");
         y1 = keyboard.nextInt();
         
         System.out.print ("Enter x2: ");
         x2 = keyboard.nextInt();
         
         System.out.print ("Enter y2: ");
         y2 = keyboard.nextInt();
         
         slope = ((y1 - y2) / (x1 - x2));
         
         System.out.println ("Coordinate 1: (" + x1 + ", " + y1 + ")");
         System.out.println ("Coordinate 2: (" + x2 + ", " + y2 + ")");
         System.out.println ("Slope: " + slope);
         
     }//End main
 }//End class

2.9

/**
 * Teresa Boehnke
 * 9/7/2017
 * Sphere
 * */
 
 import java.util.Scanner;
 import java.text.DecimalFormat;
 
 public class Sphere
 {
     // Calculates the surface area and volume of a circle given its radius
     
     public static void main (String[]args)
     {
         int radius;
         double surfaceArea, volume;
         Scanner scan = new Scanner(System.in);
         
         System.out.print ("Enter the circle's radius: ");
         radius = scan.nextInt();
         
         surfaceArea = 4* Math.PI *Math.pow(radius, 2);
         volume = (4/3) * Math.PI * Math.pow(radius, 3);
         
         // Round the output to four decimal places
         DecimalFormat fmt = new DecimalFormat ("0.####");
         
         // Output results with labels
         System.out.println ("The circle's surface area: " + fmt.format(surfaceArea));
         System.out.println ("The circle's volume: " + fmt.format(volume));
         
     }//End main
 }//End class

2.10

/**
 * Teresa Boehnke
 * 9/5/2017
 * Triangle
 * */
 
 import java.util.Scanner;
 import java.text.DecimalFormat;
 
 public class Triangle
 {
     // Calculates the area of a triangle
     
     public static void main (String[]args)
     {
         int a, b, c;
         double area, s;
         Scanner scan = new Scanner(System.in);
         
         System.out.print ("Enter the side 1: ");
         a = scan.nextInt();
         
         System.out.print ("Enter the side 2: ");
         b = scan.nextInt();
         
         System.out.print ("Enter the side 3: ");
         c = scan.nextInt();
         
         s = (a + b + c)/2;
         
         area = Math.sqrt (s * (s-a) * (s-b) * (s-c));
         
         // Round the output to three decimal places
         DecimalFormat fmt = new DecimalFormat ("0.###");
         // Output results with labels
         System.out.println ("The triangle's area: " + fmt.format(area));

         
     }//End main
 }//End class

Extra

/**
 * Teresa Boehnke
 * 9/8/2017
 * CoinCount
 * */
 
 import java.util.Scanner;
 import java.text.NumberFormat;
 
 public class CoinCount
 {
     
     public static void main (String[]args)
     {
         double q, d, n, p;
         double quarters, dimes, nickels, pennies, total;
         Scanner scan = new Scanner(System.in);
         
         System.out.print ("Enter amount of quarters: ");
         q = scan.nextInt();
         quarters = q *.25;
         
         System.out.print ("Enter amount of dimes: ");
         d = scan.nextInt();
         dimes = d *.1;
         
         System.out.print ("Enter amount of nickles: ");
         n = scan.nextInt();
         nickels = n *.05;
         
         System.out.print ("Enter amount of pennies: ");
         p = scan.nextInt();
         pennies = p *.01;
         
         total = quarters + dimes + nickels + pennies;
         
         NumberFormat money = NumberFormat.getCurrencyInstance();
         
         // Output results with labels
         System.out.println ("Total in quarters: " + quarters);
         System.out.println ("Total in dimes: " + dimes);
         System.out.println ("Total in nickels: " + nickels);
         System.out.println ("Total in pennies: " + pennies);
         System.out.println ("Total: " +money.format(total));
         

         
     }//End main
 }//End class

