# Designing-Custom-Random-PRNG-Algorithm
GitHub Subdirectory Details :
Folder Structure

Main.java

CustomRandom.java

README.md
Class Name

CustomRandom

Method Name (same name)

methodName() → overloaded

How to Use

CustomRandom.methodName(100) → random int (0–99)

CustomRandom.methodName(50, 100) → random int (range)

CustomRandom.methodName() → random double (0–1)

CustomRandom.methodName(10.0, 20.0) → random double (range)

CustomRandom.methodName(0.5f) → random float

CustomRandom.methodName(true) → random boolean

CustomRandom.methodName('A') → random A–Z character

 Mathematical Details:

Algorithm: XOR-Shift

Steps:

seed = seed XOR (seed << 13)

seed = seed XOR (seed >> 7)

seed = seed XOR (seed << 17)

New seed = random-like value

Purpose:

Built-in Random not used

Method overloading + class method used
