//# Difference-Array-ArrayList
//This code is a simple explanation of how an array and arraylist differ in Java


import java.util.ArrayList; // adding the import to be able to use the ArrayList data structure


public class DifferenceArrayArrayList {
    public static void main(String[] args) {
        System.out.println("*** This is an example of an array ***");

        double[] values = new double[10]; // Declaring an array data type that holds doubles. The size of the array is 10

        // Using the for loop to put my array example to the test. Using values.length to run through the for loop the correct number of iterations.
        for(int i = 0; i < values.length; i++){
            values[i] = (2*i)*3.14; // i will go through each element storing a value inside
            System.out.println(values[i]); // printing out each element and the value stored inside
        }


        System.out.println("*** This is an example of an ArrayList ***");

        ArrayList<String> count = new ArrayList<String>(); // Initializing the ArrayList that holds the String data type with size 0
        count.add("One"); // Increasing count to size 1 and adding element One
        count.add("Two"); // Increasing count to size 2 and adding element Two

        System.out.println(count); // Printing out the elements of the arraylist

        count.set(1, "Three"); // Keeping the arraylist at size 2 but changing element 1 to Three by using set

        System.out.println(count);
    }
}
