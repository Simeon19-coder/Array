import java.util.*;
public class ArrayScript{
    public static void main(String[] args){
        Scanner scan = new Scanner(System.in);
        String[] students = new String[10];
        double[] grades = new double[10];
        
        double sum = 0;

        System.out.println("Enter a 10 Students and their Grades.");

        for(int x=0; x<10; x++){
            System.out.println("Student" + " "+(x + 1)+" "+ "Name: ");
            students[x]=scan.nextLine();
        
            System.out.println("Grade: ");
            grades[x]=scan.nextDouble();
            scan.nextLine();
            sum += grades[x];
        }

        double ave= sum/10;
        System.out.println("\nAverage: "+ave);

        for(int x=0; x<grades.length -1; x++){
            for(int j=0; j < grades.length -x -1; j++){
                if (grades[j]>grades[j +  1]){

                    double temp =grades[j];
                    grades[j]= grades[j+1];
                    grades[j+1]=temp;
                }
            }
        }

        System.out.println("\nSorted Student Grades:");
        for(int x=0; x<10; x++){
            System.out.println(students[x] +" : "+ grades[x]);
        } 

        System.out.println("Enter Name to Search for Students: ");
        String search=scan.nextLine(); 

        boolean negate = false;

        for(int x=0; x<students.length; x++){
            if(students[x].equalsIgnoreCase(search)){
                System.out.println("Student Found!");
                System.out.println("Name: "+ students[x]);
                System.out.println("Grade: "+ grades[x]);
                negate=true;
                break;
            }
            
            }if(!negate){
                System.out.println("No Student Found!");

        }



         
    }

}