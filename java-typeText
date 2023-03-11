import java.awt.*;
import java.awt.event.KeyEvent;
import java.util.*;

class robot {
    public static void sleep(long ms) {
        try {Thread.sleep(ms);} catch (Exception ignored) {}
    }
    public static void typeText(Robot robot, String str, int n) {
        for( int j=0; j<n; j++){
            for (int i = 0; i < str.length(); i++) {
                robot.keyPress(Character.toUpperCase(str.charAt(i)));
                sleep(200);
            }
            robot.keyPress(KeyEvent.VK_ENTER);
        }
    }

    public static void main(String[] args) throws Exception {
        System.out.println("give the path of the app");
        Scanner reader = new Scanner(System.in);
        String command = reader.nextLine();

        System.out.println("give the text to automate :");
        Scanner reader1 = new Scanner(System.in);
        String str = reader1.nextLine();

        System.out.println();
        System.out.println("how many times do u wanna write that text :");
        Scanner reader2 = new Scanner(System.in);
        int n = reader2.nextInt();


        Runtime.getRuntime().exec(command);

        sleep(2000);

        Robot robot = new Robot();

        if(n == 0) {
            str = "wow,you are so clever,oh wait...";
            n = 1;
        }
        if(n== 69){
            str="nice";
            n=1;
        }
        typeText(robot, str, n);
    }
}
