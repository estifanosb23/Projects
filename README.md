import java.util.*;

public class BMIcalculator {
    public static void main(String[] args) {
        Scanner console = new Scanner(System.in);

        System.out.println("This program reads data for two people and");
        System.out.println("computes their body mass index (BMI). \n");

        System.out.println("Enter next person's information:");
        System.out.print("height (in inches) ? ");
        double height = console.nextDouble();
        System.out.print("weight (in pounds) ? ");
        double weight = console.nextDouble();


        System.out.println("\nEnter next person's information:");
        System.out.print("height (in pounds) ? ");
        double height2 = console.nextDouble();
        System.out.print("weight (in pounds) ? ");
        double weight2 = console.nextDouble();

        double BMI = (weight / (height * height)) * 703;
        System.out.print("Person 1 BMI = " + BMI);
        if (BMI < 18.5) {
            System.out.print("\nunderweight");
        }
        if (BMI >= 18.5 && BMI <= 24.9) {
            System.out.print("\nnormal");
        } 
        if (BMI >= 25.0 && BMI <= 29.9) {
            System.out.print("\noverwight");
        } 
        if (BMI >= 30) {
            System.out.print("\nobese");
        }

        double BMI2 = (weight2 / (height2 * height2)) * 703;
        System.out.print("\nPerson 2 BMI = " + BMI2);
        if (BMI2 < 18.5) {
            System.out.print("\nunderweight");
        }
        if (BMI2 >= 18.5 && BMI2 <= 24.9) {
            System.out.print("\nnormal");
        } 
        if (BMI2 >= 25.0 && BMI2 <= 29.9) {
            System.out.print("\nnormal");
        }
        if (BMI2 > 30) {
            System.out.print("\nobese");
        }
        double difference = BMI - BMI2;
        System.out.print("\nDifference = " + difference);
    }
    
}
