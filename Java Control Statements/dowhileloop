// 1) SumClass: sums 1 + 0.9 + 0.8 + ... until 0.1 using do-while
class SumClass {
    static double sumSeries() {
        double sum = 0.0;
        double term = 1.0;
        do {
            sum += term;
            term -= 0.1;
        } while (term >= 0.1);
        return sum;
    }
}

// 2) DivisorMultipleClass: computes GCD and LCM with static methods
class DivisorMultipleClass {
    public static int gcd(int a, int b) {
        while (b != 0) {
            int temp = b; b = a % b; a = temp;
        }
        return a;
    }
    public static int lcm(int a, int b) {
        return (a * b) / gcd(a, b);
    }
}

// 3) NumberConversionClass: converts between binary, decimal, hex, and octal
class NumberConversionClass {
    public static String decimalToBinary(int dec) { return Integer.toBinaryString(dec); }
    public static String decimalToHex(int dec) { return Integer.toHexString(dec); }
    public static String decimalToOctal(int dec) { return Integer.toOctalString(dec); }
    public static int binaryToDecimal(String bin) { return Integer.parseInt(bin, 2); }
    public static int hexToDecimal(String hex) { return Integer.parseInt(hex, 16); }
    public static int octalToDecimal(String oct) { return Integer.parseInt(oct, 8); }
}

// 4) CustomPrintClass: simple print method
class CustomPrintClass {
    public void pr(String message) {
        System.out.println(message);
    }
}

// 5) MainClass: creates objects and calls methods demonstrating do-while usage
public class MainClass {
    public static void main(String[] args) {
        CustomPrintClass printer = new CustomPrintClass();
        
        // SumClass usage
        double sumResult = SumClass.sumSeries();
        printer.pr("Sum of series: " + sumResult);

        // DivisorMultipleClass usage
        int a = 24, b = 36;
        printer.pr("GCD of " + a + " and " + b + ": " + DivisorMultipleClass.gcd(a, b));
        printer.pr("LCM of " + a + " and " + b + ": " + DivisorMultipleClass.lcm(a, b));
        
        // NumberConversionClass usage
        int decimal = 45;
        String binary = NumberConversionClass.decimalToBinary(decimal);
        String hex = NumberConversionClass.decimalToHex(decimal);
        String octal = NumberConversionClass.decimalToOctal(decimal);
        printer.pr("Decimal " + decimal + " to Binary: " + binary);
        printer.pr("Decimal " + decimal + " to Hex: " + hex);
        printer.pr("Decimal " + decimal + " to Octal: " + octal);

        // Demonstrate do-while loop example: counting down
        int count = 5;
        do {
            printer.pr("Count is: " + count);
            count--;
        } while (count > 0);
    }
}
