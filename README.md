## bank_system_without_oop.py

balance = 1000

def check_balance():
    print("Current Balance:", balance)

def deposit(amount):
    global balance
    balance += amount
    print("Deposited:", amount)

def withdraw(amount):
    global balance
    if amount > balance:
        print("Insufficient Balance")
    else:
        balance -= amount
        print("Withdrawn:", amount)

while True:
    print("\n1.Check Balance  2.Deposit  3.Withdraw  4.Exit")
    choice = input("Enter choice: ")

    if choice == "1":
        check_balance()
    elif choice == "2":
        amt = int(input("Enter amount: "))
        deposit(amt)
    elif choice == "3":
        amt = int(input("Enter amount: "))
        withdraw(amt)
    elif choice == "4":
        break
    else:
        print("Invalid choice") Python-project
This repository demonstrates the difference between procedural programming and object-oriented programming in Python.
