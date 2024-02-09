# Below is a Python program that simulates a simple banking system.
# A data structures like dictionaries and lists to store information about bank accounts and transactions were utilised.
# The program includes functions to create accounts, deposit and withdraw funds, transfer money between accounts, and generate account statements.

class Bank:
    def __init__(self):
        self.accounts = {}

    def create_account(self, account_number, initial_balance=0):
        if account_number in self.accounts:
            print("Account already exists.")
        else:
            self.accounts[account_number] = initial_balance
            print("Account created successfully with the name Sadiya Ahmad Mohammad.")

    def deposit(self, account_number, amount):
        if account_number in self.accounts:
            self.accounts[account_number] += amount
            print("Deposit successful. Current balance:", self.accounts[account_number])
        else:
            print("Account does not exist.")

    def withdraw(self, account_number, amount):
        if account_number in self.accounts:
            if self.accounts[account_number] >= amount:
                self.accounts[account_number] -= amount
                print("Withdrawal successful. Current balance:", self.accounts[account_number])
            else:
                print("Insufficient funds.")
        else:
            print("Account does not exist.")

    def transfer(self, from_account, to_account, amount):
        if from_account in self.accounts and to_account in self.accounts:
            if self.accounts[from_account] >= amount:
                self.accounts[from_account] -= amount
                self.accounts[to_account] += amount
                print("Transfer successful.")
            else:
                print("Insufficient funds.")
        else:
            print("One or both accounts do not exist.")

    def account_statement(self, account_number):
        if account_number in self.accounts:
            print("Account Statement for Account Number:", account_number)
            print("Current Balance:", self.accounts[account_number])
        else:
            print("Account does not exist.")


def main():
    bank = Bank()

    # Create accounts
    bank.create_account("123456", 1000000)
    bank.create_account("789012", 5000000)

    # Deposit funds
    bank.deposit("123456", 2000000)
    bank.deposit("789012", 3000000)

    # Withdraw funds
    bank.withdraw("123456", 1000000)
    bank.withdraw("789012", 2000000)

    # Transfer funds
    bank.transfer("123456", "789012", 1500000)

    # Print account statements
    bank.account_statement("123456")
    bank.account_statement("789012")


if __name__ == "__main__":
    main()

print ('Thank you for banking with us'
