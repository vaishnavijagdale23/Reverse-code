
#include <stdio.h>  // Include standard input-output header
// Function to calculate the sum of two voltages using pointers
void sumVoltages(float *voltage1, float *voltage2, float *sum) {
    *sum = *voltage1 + *voltage2;  // Sum the two voltages
}
int main() 
{

    float voltage1 = 5.5;  // First voltage value
    float voltage2 = 3.2;  // Second voltage value
    float sum;             // Variable to store the sum of the voltages

    // Pointers to the voltage values
    float *v1_ptr = &voltage1;
    float *v2_ptr = &voltage2;
    float *sum_ptr = &sum;

    // Display the given voltage values
    printf("Voltage 1: %.2f V\n", *v1_ptr);
    printf("Voltage 2: %.2f V\n", *v2_ptr);

    // Call the function to calculate the sum using pointers
    sumVoltages(v1_ptr, v2_ptr, sum_ptr);

    // Display the sum of the voltages
    printf("Sum of Voltages: %.2f V\n", *sum_ptr);

    return 0;
}


Output:
Voltage 1: 5.50 V
Voltage 2: 3.20 V
Sum of Voltages: 8.70 V

--------------------------------
Process exited after 2.686 seconds with return value 0
Press any key to continue . . .

# Reverse-code
