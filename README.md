🔥 Day 12 Python Project

🛒 Smart Euro Converter & Price Filter for Store Items

By: Geraldo Dieterle
Date: Friday, July 11


---

📌 Project Description:

This Python script simulates a small store inventory system that:

1. Converts prices from USD to EUR (using a rate of 0.85)


2. Filters items based on a minimum Euro price input from the user


3. Sorts the filtered items by their Euro price in ascending order


4. Displays results in a clean and readable way



It uses real-world logic like currency conversion, customer filtering, and list sorting — perfect for marketplaces or budget apps.


---

✅ Key Python Skills Used:

map() + lambda: to apply currency conversion to all items

filter() + lambda: to keep only items above a price

sorted() + lambda: to sort by item price

round(): to keep prices clean

input(): for dynamic user control

Tuples + Lists for data storage



---

🧠 How It Works:

store = [("Milk", 19.00), ("Meat", 45.77), ...]  # store items with USD prices

to_euros = lambda item: (item[0], round(item[1] * 0.85, 2))  # convert to EUR
store_euros = list(map(to_euros, store))

min_price = float(input("💰 What’s the minimum price in Euros? "))  # user input

price_filter = lambda item: item[1] >= min_price  # keep if price >= min
filtered = list(filter(price_filter, store_euros))

sorted_filtered = sorted(filtered, key=lambda item: item[1])  # sort by price

# Display results
for item in sorted_filtered:
    print(item)


---

🧪 Sample Output:

💰 What’s the minimum price of items in Euros? 20

Items priced at or above € 20.0

('Juice', 21.25)
('Meat', 38.91)


---

📦 Real Use Ideas:

E-commerce filters

Marketplaces

Currency-based inventory sorting

Budget tools that convert and filter items
