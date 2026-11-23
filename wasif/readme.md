Wasif this is your coding folder, Ill tell you what you need todo and attatch it and commit it in your own branch below.

Week 1:

File 1: Weapon.java

Create a class representing a hero's weapon.
• Fields: name (String), damage (int), element (String).
• Constructors:
	• Weapon(String name, int damage, String element) — sets all fields.
	• Weapon(String name, int damage) — chains to the full constructor using this(...), setting element to "Physical".
	• Weapon() — chains to the 2-argument constructor, setting name to "Rusty Dagger" and damage to 5.
• Method: getInfo() — returns a clean String like "Excalibur (50 Light DMG)".

File 2: Character.java (Base Class)

Create a base class for any living entity in the game.
• Fields: name (String), level (int), maxHealth (int).
• Constructors:
	• Character(String name, int level, int maxHealth) — sets all fields.
	• Character(String name) — chains to the full constructor, setting level to 1 and maxHealth to 100.
• Getters: Add getName(), getLevel(), and getMaxHealth().

File 3: Hero.java (Subclass of Character)

Extend Character to represent a playable hero who carries a Weapon and has gold.
• Fields: heroClass (String), gold (int), equippedWeapon (Weapon).
• Constructors:
	• Full Constructor: Hero(String name, int level, int maxHealth, String heroClass, int gold, Weapon equippedWeapon) — calls super(...) and sets the hero's fields.
	• Starter Hero Constructor: Hero(String name, String heroClass) — chains to the full constructor using this(...), defaulting level to 1, maxHealth to 100, gold to 50, and creating a new Weapon() (the default Rusty Dagger).
	• Copy Constructor: Hero(Hero other) — creates a new Hero with the exact same stats and a fresh copy of their Weapon.
• Method: printCharacterSheet() — prints all character and weapon details neatly to the console.

File 4: GameLauncher.java (Main Runner)

Write a main method that brings everything together:
1. Create a custom weapon ("Flame Sword", 35, "Fire") and a basic weapon ("Wooden Bow", 12).
2. Create three heroes using all three Hero constructors (a custom high-level hero, a brand-new starter hero, and a clone of the custom hero).
3. Print out all three character sheets to verify your defaults and chaining worked.
