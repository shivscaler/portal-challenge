Challenge Description:
In this coding challenge, you'll embark on an epic journey that combines the worlds of Marvel superheroes and the Chronicles of Narnia. Your task is to write a Python program that simulates a portal device that can transport Marvel characters into the magical land of Narnia.

Your program should achieve the following:

1. Create a Python class named `PortalDevice` that has the following methods:

- `__init__(self)`: Initializes the portal device with default values.

- `add_marvel_character(self, character_name)`: Adds a Marvel character to the portal device.

- `transport_to_narnia(self)`: Transports all added Marvel characters to Narnia.

- `list_characters_in_narnia(self)`: Lists all the Marvel characters currently in Narnia.

- `clear_narnia(self)`: Removes all Marvel characters from Narnia.

2. Create a Python class named `NarniaLand` that has the following methods:

- `__init__(self)`: Initializes Narnia with an empty list of characters.

- `accept_marvel_characters(self, characters)`: Accepts a list of Marvel characters and brings them into Narnia.

- `list_characters(self)`: Lists all the characters currently in Narnia.

You need to ensure that:

- The `PortalDevice` can hold a maximum of 10 Marvel characters at a time.
- When you transport characters to Narnia, they are removed from the portal device and added to Narnia.
- When you clear Narnia, all characters are removed from Narnia.
- The `list_characters` method of `NarniaLand` displays the names of all characters currently in Narnia.

Here's an example of how to use the classes:

```
# Create a portal device
portal = PortalDevice()

# Add Marvel characters to the portal device
portal.add_marvel_character("Spider-Man")
portal.add_marvel_character("Iron Man")
portal.add_marvel_character("Thor")

# Transport characters to Narnia
portal.transport_to_narnia()

# Create Narnia
narnia = NarniaLand()

# Accept Marvel characters into Narnia
narnia.accept_marvel_characters(portal.list_characters_in_narnia())

# List characters in Narnia
print("Characters in Narnia:", narnia.list_characters())

# Clear Narnia
narnia.clear_narnia()

# List characters in Narnia after clearing
print("Characters in Narnia after clearing:", narnia.list_characters())
```


Your challenge is to implement the `PortalDevice` and `NarniaLand` classes and test them using the provided example. Make sure the program handles the specified requirements and provides the expected output.
