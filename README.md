class BankAccount:
    def __init__(self, owner, balance=0):
        self.owner = owner
        self.balance = balance

    def deposit(self, amount):
        if amount > 0:
            self.balance += amount
            print(f"Katathesi {amount} € epituxhs.")
        else:
            print("Mh egkuro poso katathesis.")

    def withdraw(self, amount):
        if amount <= self.balance:
            self.balance -= amount
            print(f"Analhpsh {amount}€ epituxhs.")
        else:
            print("Aneparkses ypoloipo.")

    def show_balance(self):
        print(f"Owner: {self.owner}")
        print(f"Balance: {self.balance}€")



account1 = BankAccount("Giwrgos", 500)
account2 = BankAccount("Elenh", 1000)


account1.deposit(200)
account1.withdraw(100)
account1.show_balance()

print("---------------")

account2.withdraw(300)
account2.show_balance()
