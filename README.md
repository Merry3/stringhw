# stringHW


import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
      System.out.println(" Please fill the following form");

      Scanner userInput=new Scanner(System.in);
      System.out.println("Please Enter your Monthly Salary");
        int salary=userInput.nextInt();

        System.out.println("Enter your Bank Saving Amount (Number only)");
        int saving=userInput.nextInt();

        System.out.println("Do you have a criminal record? True/False ");
        String criminalRecord= userInput.nextLine();


        System.out.println("How many monthly socialscore do you have?");
        int socialScore=userInput.nextInt();

        String status1= ( salary >70000)?"True":"False";
        String status2= ( saving >5000000)?"True":"False";
        String status3= (( socialScore*12) <55 )?"True":"False";

        String credit=((status2)&&(status1)&&(criminalRecord && status3)? "CONGRADULATIONS YOU CAN BORROW THE MONEY!":"SORRY YOU CANNOT BORROW MONEY FROM OUR BANK";
        System.out.println(credit);
....................//..............................................//...........................................//.....................................//.....................import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
      System.out.println(" Please fill the following form");

      Scanner userInput=new Scanner(System.in);
      System.out.println("Please Enter your Monthly Salary");
        int salary=userInput.nextInt();

        System.out.println("Enter your Bank Saving Amount (Number only)");
        int saving=userInput.nextInt();

        System.out.println("Do you have a criminal record? True/False ");
        boolean criminalRecord= userInput.nextBoolean();


        System.out.println("How many monthly socialscore do you have?");
        int socialScore=userInput.nextInt();


       boolean  status1 = Boolean.parseBoolean(salary>70000? "True": "false");
        boolean  status2 = Boolean.parseBoolean(saving>5000000 ? "True": "false");
        boolean status4= Boolean.parseBoolean(((socialScore*12) <55?"True":"False"));
        //boolean credit=(status1 && status2)&&(crmrecod||status4 ) =;
        String credit=((status1 && status2)&&(criminalRecord||status4 ))? "CONGRADULATIONS YOU CAN BORROW THE MONEY!":"SORRY YOU CANNOT BORROW MONEY FROM OUR BANK" ;
       System.out.println(credit);





    }
}


