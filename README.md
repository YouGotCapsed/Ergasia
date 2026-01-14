
class BankAccount:
    def __init__(self, owner, balance=0):
        self.owner = owner
        self.balance = balance

    def deposit(self, amount):
        if amount > 0:
            self.balance += amount
            print(f"Κατάθεση {amount}€ επιτυχής.")
        else:
            print("Μη έγκυρο ποσό κατάθεσης.")

    def withdraw(self, amount):
        if amount <= self.balance:
            self.balance -= amount
            print(f"Ανάληψη {amount}€ επιτυχής.")
        else:
            print("Ανεπαρκές υπόλοιπο.")

    def show_balance(self):
        print(f"Ιδιοκτήτης: {self.owner}")
        print(f"Υπόλοιπο: {self.balance}€")



account1 = BankAccount("Γιώργος", 500)
account2 = BankAccount("Ελένη", 1000)


account1.deposit(200)
account1.withdraw(100)
account1.show_balance()

print("---------------")

account2.withdraw(300)
account2.show_balance()
