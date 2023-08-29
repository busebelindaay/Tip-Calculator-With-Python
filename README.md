# Tip-Calculator-With-Python
#The code calculates amount of the tip and adds on the bill. After that it prints the total amount of each person for paying.

print("Welcome to the tip calculator")
total_bill = float(input("What was the total bill?"))
percentage_tip = float(input("What percentage tip would you like to give? 10, 12 or 15?"))
numbers_of_people = float(input("How many people to split the bill?"))

bills_amount_of_each_person = ((percentage_tip / 100) * total_bill + total_bill) / numbers_of_people

final_amount = "{:.2f}".format(bills_amount_of_each_person)

print(f"Each person should pay: ${final_amount} ")
