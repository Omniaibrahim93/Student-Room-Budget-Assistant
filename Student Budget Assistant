# Student Budget Assistant
# Author: Omnia Ibrahim
# Date: July 2025
# Description:
# This program helps students track their monthly expenses based on a user-defined budget.
# It collects spending in 5 categories, calculates totals, and gives feedback based on usage.

def get_float_input(prompt):
    """
    Reusable function to get numeric input from user.
    If input is invalid, it keeps asking until a valid number is entered.
    """
    while True:
        try:
            return float(input(prompt))
        except ValueError:
            print("⚠️ Please enter a valid number.")

# 1. Greet the student and get their name
print("Welcome to your Smart Budget Assistant! 🎓")
student_name = input("What is your name? ")

# 2. Ask for the student's monthly budget
monthly_budget = get_float_input(f"Hi {student_name}, what is your monthly budget? AED ")

# 3. Ask for expenses in each category
print("\nPlease enter your expenses for the following categories:")
food_expense = get_float_input("🍔 Food: AED ")
transport_expense = get_float_input("🚌 Transport: AED ")
housing_expense = get_float_input("🏠 Rent or Housing: AED ")
internet_expense = get_float_input("🌐 Internet & Utilities: AED ")
entertainment_expense = get_float_input("🎮 Entertainment: AED ")

# 4. Calculate total spent and remaining balance
total_spent = food_expense + transport_expense + housing_expense + internet_expense + entertainment_expense
remaining = monthly_budget - total_spent

# 5. Display results
print("\n📊 Budget Summary:")
print(f"Total Spent: AED {round(total_spent, 2)}")
print(f"Remaining Balance: AED {round(remaining, 2)}")

# 6. Show budget status with motivation
if total_spent < monthly_budget * 0.9:
    print("✅ You're within budget! Keep up the smart spending! 💪")
elif total_spent <= monthly_budget:
    print("⚠️ Warning: You're approaching your budget limit. Spend carefully.")
else:
    print("❌ You’ve exceeded your budget. Be cautious with your remaining expenses! 🧠")

# 7. Closing message
print(f"\nThank you for using the Budget Assistant, {student_name}! 💡")
