import Float "mo:base/Float";
import Debug "mo:base/Debug";

actor ExamAverageCalculator {
    public func calculateAverage(exam1 : Float, exam2 : Float) : async Float {
        let sum = exam1 + exam2;
        let average = sum / 2;
        
        Debug.print("Exam 1 result: " # Float.toText(exam1));
        Debug.print("Exam 2 result: " # Float.toText(exam2));
        Debug.print("Average: " # Float.toText(average));
        
        average
    };
}#
