phonebook = {}

def add_phone_number():
    """Prompt user to enter a phone number and contact name, then save it."""
    phone_number = input("Enter phone number: ")
    contact_name = input("Enter contact name: ")
    phonebook[contact_name] = phone_number
    print(f'Phone number {phone_number} added for contact {contact_name}.')

def view_saved_numbers():
    """Display all saved phone numbers and their associated names."""
    if not phonebook:
        print('No phone numbers saved.')
    else:
        print("Saved phone numbers:")
        for name, number in phonebook.items():
            print(f'{name}: {number}')

def delete_contact():
    """Prompt user to enter a contact name to delete, then remove it."""
    contact_name = input("Enter the contact name to delete: ")
    if contact_name in phonebook:
        del phonebook[contact_name]
        print(f'Contact {contact_name} deleted.')
    else:
        print(f'Contact {contact_name} not found.')

while True:
    print("\nPhonebook Menu:")
    print("1. Add a phone number")
    print("2. View saved phone numbers")
    print("3. Delete a contact")
    print("4. Exit")

    choice = input("Enter your choice (1-4): ")

    if choice == '1':
        add_phone_number()
    elif choice == '2':
        view_saved_numbers()
    elif choice == '3':
        delete_contact()
    elif choice == '4':
        break
    else:
        print("Invalid choice. Please enter a number between 1 and 4.")
