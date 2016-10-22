# Awesome-Calculator
You are to build a browser based calculator with the following requirements:

1. The calculator must support at least the following operations: +, -, *(multiplication), /, **(exponentiation), sqrt
2. The calculator must store the last 10 calculations performed by the user.  The list of calculations must survive a refresh but not necessarily a cookie clear.  The list should be tied to the browser that performed the calculation.  In other words, if a user performs a calculation on Browser A, and then performs a calculation on Browser B, when the app is accessed from Browser A only calculations performed from Browser A should appear and vice versa.
3. The calculator should be able to handle arbitrary precision floats(a "BigDecimal" type)
4. Calculations may be performed on the server or the client side.  However, no reloading of the page is allowed
5. Aesthetics are important but not as important as satisfying the criteria listed above.


The implementation I made stores the values when the "=" button is pressed. Exponentiation is basically operand ^ power and the sqrt button is applied to the previous operand entered and is internally translated to operand ^ 0.5 which is the same thing.
The values stored are per window/tab and survive refresh/cookie clear but not the closing of the window/tab.
