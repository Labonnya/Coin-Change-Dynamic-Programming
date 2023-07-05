# Dynamic-Programming

Code Description:

This code implements a dynamic programming approach to solve the minimum coin change problem. Given a target amount 'n' and a set of coins with different denominations, the code determines the minimum number of coins required to make change for the target amount.

The main function 'minCoin' takes three parameters:
1. 'a' - an array representing the available denominations of coins.
2. 'n' - the target amount for which the minimum number of coins needs to be determined.
3. 'dp' - an array used for memoization to store previously calculated results.

The code utilizes a recursive approach with memoization to avoid redundant calculations. It iterates through each coin denomination and recursively calculates the minimum number of coins required for the remaining amount by subtracting the current coin's denomination from the target amount. The minimum value obtained from these recursive calls is then stored in the 'dp' array for future reference.

The main function initializes the 'dp' array with -1, except for the base case where dp[0] is set to 0, representing that no coins are needed to make change for 0 amount.

The user is prompted to input the total money 'n', the number of available coins 'x', and the denominations of the coins. The 'minCoin' function is called with the input values, and the result (minimum number of coins required) is stored in the variable 'lab'. Finally, the code displays the minimum number of coins required to make change for the given amount.

Note: The code assumes that the denominations of coins are provided in non-decreasing order.
