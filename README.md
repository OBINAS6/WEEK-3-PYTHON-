# WEEK-3-PYTHON-
def calculate_discount(price, discount_percent):
    # Check if the discount is 20% or higher
    if discount_percent >= 20:
        # Apply the discount
        final_price = price - (price * discount_percent / 100)
        return final_price
    else:
        # Return the original price if no discount is applied
        return price

# Prompt the user for input
price = float(input("Enter the original price of the item: "))
discount_percent = float(input("Enter the discount percentage: "))

# Call the function and print the result
final_price = calculate_discount(price, discount_percent)

# Print the final price or the original price
if final_price == price:
    print(f"No discount applied. The original price is: ${final_price:.2f}")
else:
    print(f"The final price after applying the discount is: ${final_price:.2f}")
