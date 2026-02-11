# Shopping-cart-program-0239
Simple shopping cart program lol
import time

print("you are going to the supermarket")
time.sleep(3)
print("you've arrived at the supermarket")
time.sleep(2)
print("you picked up a shopping cart")
time.sleep(1)
items = []
prices = []
total = 0
while True:
    item_ = input("Put the item you like into your shopping cart(c to checkout): ")
    if item_.lower() == "c":
        for price in prices:
           total += price
        print(f"your total is {total}")
        print(f"you bought {items}")
        break
    else:
        price = float(input(f"enter the price of the {item_}: "))
        items.append(item_)
        prices.append(price)
        print(f"shopping cart: {items}")
        
