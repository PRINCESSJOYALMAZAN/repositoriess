import java.util.Scanner;

public class EmotionalRecognitionDevice {

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.println("Welcome to Emotional Recognition Device");

        // Simulate detecting mood
        int mood = detectMood(scanner);
       
        // Simulate measuring blood pressure
        double bloodPressure = measureBloodPressure(scanner);
       
        // Coping mechanisms based on mood
        copeWithMood(mood);
       
        // Simulate processing data
        processData(mood, bloodPressure);
       
        System.out.println("Thank you for using Emotional Recognition Device");
    }

    // Simulate detecting mood
    private static int detectMood(Scanner scanner) {
        System.out.println("Please rate your mood from 1 to 10 (1 being very sad, 10 being very happy):");
        int mood = scanner.nextInt();
        return mood;
    }

    // Simulate measuring blood pressure
    private static double measureBloodPressure(Scanner scanner) {
        System.out.println("Please enter your blood pressure:");
        double bloodPressure = scanner.nextDouble();
        return bloodPressure;
    }

    // Coping mechanisms based on mood
    private static void copeWithMood(int mood) {
        if (mood >= 7) {
            System.out.println("You seem to be in a good mood. Keep it up!");
        } else if (mood >= 4) {
            System.out.println("You seem to be in an average mood. Try listening to music or going for a walk.");
        } else {
            System.out.println("You seem to be in a low mood. It's okay, take a deep breath and try to relax.");
        }
    }

    // Simulate processing data
    private static void processData(int mood, double bloodPressure) {
        System.out.println("Processing data...");
        // Here you could perform further analysis or send data to a server for more advanced processing
        System.out.println("Data processed. Mood: " + mood + ", Blood Pressure: " + bloodPressure);
    }
}
