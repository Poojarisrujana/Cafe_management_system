# Cafe_management_system
#Define the menu of Restaurant
menu= {
    'Masala puri':40,
    'Pani puri':50,
    'Burger':60,
    'Gobi':70,
    'Coffee':80,
}

#Greetings
print("Welcome to Shizuka's Restaurant")

#menu
print("Pizza: 40Rs\nPaste: 50Rs\nBurger: 60Rs\nSalad: 70Rs\nCoffee: 80Rs")

order_total = 0

while True:
    item = input("Enter the name of item you want to order = ")
    if item in menu:
        order_total += menu[item]
        print(f"Your item {item} has been added to your order")
    else:
        print("Sorry, we don't have that item on the menu")


#Another item or Order
    another_order = input("Do you want to add another item? (Yes/No)")
    if another_order != "Yes":
        break
print(f"The total amount of items to pay is {order_total} Rs")
