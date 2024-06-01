package miniproject;
import java.util.Scanner;


class Password {
    String num;
    Scanner sc = new Scanner(System.in);

    void check() {
        System.out.println("Enter the password");
        num = sc.nextLine();
        int length = num.length();

        boolean hasLower = false, hasUpper = false, hasDigit = false, hasSpecial = false;
        String specialCharacters = "&@#";

        if (length >= 8) {
            for (int i = 0; i < length; i++) {
                char ch = num.charAt(i);

                if (Character.isLowerCase(ch)) {
                    hasLower = true;
                } else if (Character.isUpperCase(ch)) {
                    hasUpper = true;
                } else if (Character.isDigit(ch)) {
                    hasDigit = true;
                } else if (specialCharacters.contains(Character.toString(ch))) {
                    hasSpecial = true;
                }
            }

            if (hasLower && hasUpper && hasSpecial && hasDigit) {
                System.out.println("PASSWORD IS STRONG");
            } else {
                System.out.println("PASSWORD IS NOT STRONG");
            }
        } else {
            System.out.println("PASSWORD IS NOT STRONG");
        }
    }
}

public class ques {
    public static void main(String[] args) {
        Password p = new Password();
        p.check();
    }
}
