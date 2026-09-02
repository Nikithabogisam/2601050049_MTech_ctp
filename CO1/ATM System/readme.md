Decomposition and Abstraction

ATM Withdrawal System

A customer has ₹10,000 in their bank account and wants to withdraw ₹2,000 from an ATM.

Question

How can decomposition and abstraction be applied to design a simple ATM withdrawal system?

Solution

The ATM withdrawal problem can be solved using Decomposition and Abstraction.

Decomposition divides the withdrawal process into smaller tasks such as verifying the PIN, checking the balance, withdrawing the money, and displaying the remaining balance.

Abstraction hides the internal processing of the ATM and shows only the required information to the customer.

Example

Suppose a customer has ₹10,000 in their account and wants to withdraw ₹2,000.

Given:

Account Balance = ₹10,000

Correct PIN = 1234

Withdrawal Amount = ₹2,000

Entered PIN = 1234

1. Verify PIN

The customer enters the PIN:

Entered PIN = 1234

Correct PIN = 1234

Since both PINs are equal, the PIN is verified successfully.

2. Check Balance

Withdrawal Amount = ₹2,000

Available Balance = ₹10,000

Check:

₹2,000 ≤ ₹10,000

Since enough balance is available, the withdrawal can be processed.

3. Withdraw Money

The withdrawal amount is deducted from the account balance.

Remaining Balance:

₹10,000 − ₹2,000 = ₹8,000

Therefore:

Amount Withdrawn = ₹2,000

Remaining Balance = ₹8,000

4. Abstraction

The customer only sees the necessary information such as:

Enter PIN
Enter Withdrawal Amount
Withdrawal Successful
Remaining Balance

The internal processing of the bank account and transaction is hidden from the customer.

Algorithm

Input

Account balance

Correct PIN

Customer PIN

Withdrawal amount

Steps

Set the account balance as ₹10,000 and PIN as 1234.

Enter the PIN.

Check whether the PIN is correct.

If the PIN is correct, enter the withdrawal amount.

Check whether enough balance is available.

If yes, subtract the amount from the balance and display the remaining balance.

If no, display "Insufficient Balance".

Python Implementation

balance = 10000
correct_pin = 1234

pin = int(input("Enter PIN: "))

if pin == correct_pin:
    amount = int(input("Enter withdrawal amount: "))

    if amount <= balance:
        balance = balance - amount
        print("Withdrawal Successful")
        print("Amount Withdrawn:", amount)
        print("Remaining Balance:", balance)
    else:
        print("Insufficient Balance")
else:
    print("Invalid PIN")

Output

Enter PIN: 1234
Enter withdrawal amount: 2000
Withdrawal Successful
Amount Withdrawn: 2000
Remaining Balance: 8000

Time Complexity

Best Case

O(1)

Worst Case

O(1)
