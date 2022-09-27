import java.util.*;
import java.util.Scanner;
import java.util.Arrays;
public class Food
{
    public static void main(String[] args)
    {
        double number = 1;
        Scanner input = new Scanner(System.in);

        System.out.print("Ask me anything: " );
        String sentence = input.nextLine();

        String[] reply = {"Yes you should", "No you shouldn't"};

        int random = (int)(Math.random()*2);

        String output = reply[random];
        System.out.println( output ); //replying Yes or No

        if( output == reply[0] )// output.equals("Absolutely" ))
        {
            System.out.print("How many options would you like: ");
            int options = input.nextInt();
            input.nextLine();



                List<String> list = new ArrayList<String>();

                if( options == 5) {
                    System.out.print("Option 1: ");
                    String one = input.nextLine();

                    list.add(one);

                    System.out.print("Option 2: ");
                    String two = input.nextLine();

                    list.add(two);

                    System.out.print("Option 3: ");
                    String three = input.nextLine();

                    System.out.print("Option 4: ");
                    String four = input.nextLine();

                    System.out.print("Option 5: ");
                    String five = input.nextLine();
                }
                else if(options == 4 )
                    {
                        System.out.print("Option 1: ");
                        String one = input.nextLine();

                        list.add(one);

                        System.out.print("Option 2: ");
                        String two = input.nextLine();

                        list.add(two);

                        System.out.print("Option 3: ");
                        String three = input.nextLine();

                        System.out.print("Option 4: ");
                        String four = input.nextLine();

                    }
                else if( options == 3 )
                    {
                        System.out.print("Option 1: ");
                        String one = input.nextLine();

                        list.add(one);

                        System.out.print("Option 2: ");
                        String two = input.nextLine();

                        list.add(two);

                        System.out.print("Option 3: ");
                        String three = input.nextLine();
                    }
                else if( options == 2 )
                    {
                        System.out.print("Option 1: ");
                        String one = input.nextLine();

                        list.add(one);

                        System.out.print("Option 2: ");
                        String two = input.nextLine();
                    }
                else if( options == 1)
                    {
                        System.out.print("Option 1: ");
                        String one = input.nextLine();

                        list.add(one);
                    }
                else
                    {
                    System.out.println("WOOOOOW That's too many options!!!");
                    }

                int random1 = (int) (Math.random() * options);
                System.out.println("\nHmmm...\n            You should get " + list.get(random1));
            }


        }

    }
    
