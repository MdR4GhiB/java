# java
import java.util.Scanner;
class AreaOfShape{
    Scanner input = new Scanner(System.in);
    //This is for Rectangle area function
    void areaRectangle(){
        System.out.println("Enter length of Rectangle: ");
        float l = input.nextFloat();
        System.out.println("Enter the breadth of Rectangle: ");
        float b = input.nextFloat();
        float area = l*b;
        System.out.println("The area of Rectangle: "+area+" meter square");
    }
    //This is for Circle area find function
    void areaOfCircle(){
        System.out.println("Enter the radious: ");
        float r = input.nextFloat();
        float area = (float) (3.14*r*r);
        System.out.println("Area of Circle: "+area+" square meter");
    }
    void areaOfCylinder(){
        System.out.println("Enter the radious of cylinder: ");
        float r = input.nextFloat();
        System.out.println("Enter the height of cylinder: ");
        float h = input.nextFloat();
        float area = (float) (3.14*r*r*h);
        System.out.println("The area of cylinder is: "+area+" square meter");
    }
}
public class AreaCalculator{
    public static void main(String[]args){
        Scanner input = new Scanner(System.in);
        System.out.println("This is area calculator");
        System.out.println("-----------------------");
        System.out.println("1. Rectangle");
        System.out.println("2. Circle");
        System.out.println("3. Cylinder ");
        System.out.println("3. Exit");
        System.out.println("-----------------------");
    AreaOfShape A1 = new AreaOfShape();
    while(true){
        System.out.println("Choose one option: ");
        int choose = input.nextInt();
        switch(choose){
            case 1:
            A1.areaRectangle();
            break;
            case 2:
            A1.areaOfCircle();
            break;
            case 3:
            A1.areaOfCylinder();
            break;
            case 4:
            System.out.println("Exit..Thanks");
            return;
        }
    }

    }
}
