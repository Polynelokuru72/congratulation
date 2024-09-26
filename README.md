# Predefined names for each category
responses = {
    'Mosheneemate': ['Polyne'],
    'Best Friend': ['Ritah'],
    'Absentminded': ['Becky'],  
    'Sumbua Wake': ['Maggie'],
    'Rommies':['All']
}

while True:
    print("\nChoose a category to view:")
    for i, category in enumerate(responses.keys(), start=1):
        print(f"{i}. {category}")

    choice = input("Enter the number of your choice (or 'quit' to exit): ").strip().lower()
    
    if choice == 'quit':
        break

    if choice.isdigit() and 1 <= int(choice) <= len(responses):
        selected_category = list(responses.keys())[int(choice) - 1]
        print(f"\nThe one who is her {selected_category}: ", responses[selected_category])
    else:
        print("Invalid choice, please try again.")

print("\n CONGRATULATIONS to you Mercy!")
print("\n We love you so much")
