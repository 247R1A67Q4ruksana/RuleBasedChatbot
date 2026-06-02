# RuleBasedChatbot
import java.util.Scanner;

public class RuleBasedChatbot {

    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        System.out.println("AI Chatbot: Hello! Type 'bye' to exit.");

        while (true) {

            System.out.print("You: ");
            String input = sc.nextLine().toLowerCase();

            if (input.equals("bye")) {
                System.out.println("AI Chatbot: Goodbye! Have a great day.");
                break;
            }
            else if (input.contains("hello") || input.contains("hi")) {
                System.out.println("AI Chatbot: Hello! How can I help you?");
            }
            else if (input.contains("how are you")) {
                System.out.println("AI Chatbot: I am fine. Thank you for asking!");
            }
            else if (input.contains("your name")) {
                System.out.println("AI Chatbot: I am a Rule-Based AI Chatbot.");
            }
            else if (input.contains("help")) {
                System.out.println("AI Chatbot: You can greet me, ask my name, or type bye to exit.");
            }
            else {
                System.out.println("AI Chatbot: Sorry, I don't understand that.");
            }
        }

        sc.close();
    }
}