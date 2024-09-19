# Practica-4-Java-FizzBuzz
Crear un FizzBuzz
Usar el operador module %

1. Si es divisible entre 5 y 3, imprime FizzBuzz
2. Si es divisible entre 5, imprime Fizz
3. Si es divisible entre 3, imprime Buzz
4. Si no es divisible entre 5 y 3, imprime no es divisible entre 5 y 3
   
```java
  public class FizzBuzz {
    public static String fizzbuzz(int n) {
      /* tu codigo va aqui */
      
    }

    public static void testFizzBuzz() {
        Object[][] testCases = {
            {1, "1"},
            {2, "2"},
            {3, "Fizz"},
            {5, "Buzz"},
            {6, "Fizz"},
            {10, "Buzz"},
            {15, "FizzBuzz"},
            {30, "FizzBuzz"},
            {23, "23"}
        };
        
        for (int i = 0; i < testCases.length; i++) {
            int input = (int) testCases[i][0];
            String expected = (String) testCases[i][1];
            String result = fizzbuzz(input);
            
            if (!result.equals(expected)) {
                System.out.println("Test case " + (i + 1) + " failed: fizzbuzz(" + input + ") should be '" + expected + "', but got '" + result + "'");
            } else {
                System.out.println("Test case " + (i + 1) + " passed.");
            }
        }
    }

    public static void main(String[] args) {
        testFizzBuzz(); 
    }
}
```
