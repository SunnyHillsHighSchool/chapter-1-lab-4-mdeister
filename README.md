# Chapter-1-Lab-4

Project... Linear Function

You are a software engineer with the Blue Pelican Engineering Corporation. Your immediate
supervisor has need of a class called LinearFunction and she knows exactly the methods that it
needs to include. Not having time to write it herself, she assigns the job to you. To insure that
you produce exactly the methods she wants, she is providing the interface below and requiring
that you implement this interface in the LinearFınction class you produce. When your project is
complete, she will simply look at your class signature and if she sees implements
LinearFunctionMethods, she will know for certain that you have implemented all the methods
she originally specified in the interface; otherwise, your code would not compile

public interface LinearFunctionMethods
double getSlope()
double getYintercept();
double getRoot();

double getYvalue(double x); //return the y value corresponding to x
double getXvalue(double y); //return the x value corresponding to y

For simplicity we will assume that the linear function's graph can never be vertical or horizontal.
(This eliminates some complications with the math). In writing your methods, simply recall the y
 = mx +b portion of your algebra studies. The constructor of your class should allow you to pass
the slope (m) and y-intercept(b) of the LinearFunction object you are instantiating

Test your LinearFunction class with the Main class below:

import java.io.*
import java.util.*
public class Main
{
    public static void main(String args[])
     {
            Scanner kbReader = new Scanner(System.in);
            
System.out.print("What is the slope of your line? ");
            double slope =  kbReader.nextDouble();
             
System.out.print("What is the y-intercept of your line?");
              double yIntc =  kbReader.nextDouble();

              LinearFunction line = new LinearFunction(slope, ylntc);
              
System.out.println("The Slope of this line is:" + line.getSlope());
              
System.out.println(“Y-intercept of this line is:  “+line.getYIntercept());  
System.out.println("Root of this line is:" + line.getRoot());

               System.out.print “\nWhat is an x value for which you wish to solve for y?");
               double x = kbReader.nextDouble();
               double yValue =  line.getYvalue(x);
               System.out.println(“ The y value responding tox-x+"yVae)
               
System.out.printn(“\nWhat is a y value for which you wish to solve for x? ");
               double y  = kbReader.nextDoubl():
               double xValue = line.getXvalue(y);
                System.out.println (The x value corresponding to y = " + y + "is" +xValue):
   }
}


Below is a typical run:

What is the slope of your line?-3
What is the y-intercept of your line? 2.5

Slope of this line is -3.0
Y-intercept of this line is: 2.5
Root of this 1ine is 0.8333333333333334

What is an x value for which you wish to solve for y? -4 61
The y value corresponding to 4.61 is 16.330000000000002

What is a y value for which you wish to solve for x? 5.0
The x value corresponding to y = 5.0 is -0.833333333333334



