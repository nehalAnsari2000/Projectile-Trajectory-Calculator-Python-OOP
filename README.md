# Projectile Trajectory Calculator (Python)

## Overview
This project is part of the **Scientific Computing with Python** certification on **FreeCodeCamp**, where I learned about **Object-Oriented Programming (OOP), class inheritance, encapsulation, and data hiding in Python**. The program calculates and visualizes the trajectory of a projectile launched at a given speed, height, and angle.

The project makes use of:
- **Encapsulation** and **Data Hiding**: Private attributes (`__speed`, `__height`, `__angle`) are implemented using **name mangling**.
- **Getters and Setters**: Used to control access to private attributes securely.
- **Efficient Memory Management with `__slots__`**: Limits memory usage by restricting instance attributes.
- **Mathematical Modeling**: Implements kinematic equations to compute projectile motion.
- **Graphical Representation**: Creates a **text-based trajectory plot** using ASCII characters.
- **Table Representation**: Displays the x and y coordinates of the projectile at different points.

## Features
### 1️⃣ **Encapsulation & Data Hiding**
- The class `Projectile` hides its attributes (`speed`, `height`, `angle`) using **name mangling**.
- Uses `@property` decorators to provide controlled access to private attributes.

### 2️⃣ **Memory Optimization with `__slots__`**
- The `__slots__` mechanism is used to **restrict attribute creation** and optimize memory usage.

### 3️⃣ **Mathematical Calculation of Projectile Motion**
- Uses physics equations to compute projectile motion.
- Determines the projectile’s horizontal displacement, height at various points, and total trajectory.

### 4️⃣ **Table of Coordinates**
- Prints the calculated **x and y** coordinates of the projectile at different positions.

### 5️⃣ **Graphical Trajectory Plot**
- Uses ASCII characters to **display the projectile’s flight path**.
- `∙` represents the projectile.
- `T` represents the x-axis, and `⊣` represents the y-axis.

## Code Structure
### **Projectile Class**
- **`__slots__ = ('__speed', '__height', '__angle')`**: Restricts instance attributes for **memory efficiency**.
- **Encapsulation**: Private attributes (`__speed`, `__height`, `__angle`) ensure **data security**.
- **Getters & Setters**: Control attribute modification.
- **Mathematical methods**:
  - `__calculate_displacement()`: Computes total horizontal distance.
  - `__calculate_y_coordinate(x)`: Computes height at a given x-position.
  - `calculate_all_coordinates()`: Returns a list of all (x, y) coordinates.

### **Graph Class**
- **Stores calculated coordinates** and visualizes them.
- Methods:
  - `create_coordinates_table()`: Displays a formatted **table** of (x, y) values.
  - `create_trajectory()`: Generates an **ASCII trajectory graph**.

