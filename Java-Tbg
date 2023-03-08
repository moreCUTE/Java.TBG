
import java.util.Scanner;
import java.util.Random;
class Main {
  public static void main(String[] args) {
    Random rand = new Random();
    Scanner Doggo = new Scanner(System.in); // create this thing to get user input
   
    System.out.println("Java Text Based Game!"); //prints to screen

    //game variables
    int room = 1;
    String input = "glurbaburbal!"; //dummy value for game loop
    String[] inventory = {" ", " ", " ", " "}; //use this to hold player items
    int bag = 0;
    int rand_int1 = rand.nextInt(50);
    int rand_int2 = rand.nextInt(50);
    int rand_int3 = rand.nextInt(50);
    int rand_int4 = rand.nextInt(50);
    int rand_int5 = rand.nextInt(50);

    while (input != "quit") { //OMG GAME LOOP-----------------------------------------

      //print inventory
      System.out.println("Inventory:");
      for(int i = 0; i<=3; i++)
        System.out.println(inventory[i]);
      System.out.println("you got");
      System.out.println(bag+ "coins");
      
      switch (room) {
        case 1:
          System.out.println("You're in room 1, you can go East");
          System.out.println("you have aquired"+rand_int5+ "coins");
          
          bag=+rand_int5;
          input = Doggo.nextLine();
          if(input.equals("East"))
            room = 2;
          break;
        case 2:
          System.out.println("You're in room 2, you can go West or South");
          input = Doggo.nextLine();
          if(input.equals("South"))
            room = 3;
          else if (input.equals("West"))
            room = 1;
          break;
        case 3:
          System.out.println("You're in room 3, you can go North or West.");
          System.out.println("you have aquiored"+rand_int4+ "coins");
          bag=+rand_int4;
          //check if they already have the gun, if not tell them they got it
          if (!inventory[0].equals("marshmallow gun")){
            System.out.println("OMG you got the marshmallow gun!");
            inventory[0] = "marshmallow gun";
          }
          input = Doggo.nextLine();
          if(input.equals("North"))
            room = 2;
          else if (input.equals("West"))
            room = 4;
          break;
        case 4:
          System.out.println("You're in room 4, you can go East or West");
          input = Doggo.nextLine();
         
          if (input.equals("East"))
            room = 3;
          else if (input.equals("West"))
            room = 5;
          break;
        case 5:
          System.out.println("You are in room 5, you can go East, North, or South");
          System.out.println("you have aquired"+rand_int1+ "coins");
          bag=+rand_int1;
          input = Doggo.nextLine();
           if (!inventory[2].equals("bred")){
            System.out.println("you foidn bred");
            inventory[2] = "bred";
           }
          if (input.equals("East"))
            room = 4;
          else if (input.equals("North"))
            room = 6;
          else if (input.equals("South"))
            room = 7;
          break;
        case 6:
          System.out.println("You are in room 6, you can go South");
          System.out.println("You have found"+rand_int3 + "coins");
          bag=+rand_int3;
          input = Doggo.nextLine();
             if (!inventory[1].equals("shiny key")){
            System.out.println("you camne accross shiny key");
            inventory[1] = "shiny key";
             }
          if (input.equals("South"))
            room = 5;
          break;
        case 7:
          System.out.println("You are in room 7, you can go North or South");
          input = Doggo.nextLine();
          if (input.equals("North"))
            room = 5;
          else if (input.equals("South"))
            if (!inventory[1].equals("shiny key"))
              System.out.println("where key?");
            else
              room = 8;
          break;
        case 8:
          System.out.println("You are in room 8, you can go North");
          System.out.println("You have found"+rand_int2 + "coins");
          bag=+rand_int2;
          input = Doggo.nextLine();
           if (!inventory[3].equals("tu mama")){
            System.out.println("you find tu mama");
            inventory[3] = "tu mama";
           }
          if (input.equals("North"))
            room = 7;
          break;


      }// end bracket for switch
    } // end bracket for OMG GAME LOOP----------------------------------------------------
  }// end bracket for public static void main
}// end bracket for class main
