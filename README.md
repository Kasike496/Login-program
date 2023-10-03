import java.util.Scanner;
 public class UNIVERSITY
 {
     public static void main(String [] args)
     {
         Scanner enter=new Scanner(System.in);
         String username,password;
         int count=0;
         boolean loggedin=false;
         while(count<3)
         {
             System.out.println("enter username=");
             username=enter.nextLine();
              System.out.println("enter password=");
             password=enter.nextLine();
             System.out.println("password:");
             for(int i=0;i<password.length();i++)
             {
                 System.out.println("*");
             }
             System.out.println();
             if(username.equals("user")&&password.equals("pass"))
             {
                 loggedin=true;
                 break;
             }
             else{
                 System.out.println("incorrect username or password. please try again.");
                 count++;
             }
         }
         if(loggedin)
         {
             System.out.println("login successful!");
         }
         else
         {
             System.out.println("you have exceeded the maximum number of attempts.please try again later");
         }
     }       
 }
