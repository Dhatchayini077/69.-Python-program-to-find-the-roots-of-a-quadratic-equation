# 69.-Python-program-to-find-the-roots-of-a-quadratic-equation
import math

a = float(input("Enter the first coefficient: "))
b = float(input("Enter the second coefficient: "))
c = float(input("Enter the third coefficient: "))

if a != 0.0:
    d = (b * b) - (4 * a * c)  # discriminant

    if d == 0.0:
        print("The roots are real and equal.")
        r = -b / (2 * a)
        print("The roots are", r, "and", r)

    elif d > 0.0:
        print("The roots are real and distinct.")
        r1 = (-b + math.sqrt(d)) / (2 * a)
        r2 = (-b - math.sqrt(d)) / (2 * a)
        print("The root1 is:", r1)
        print("The root2 is:", r2)

    else:
        print("The roots are imaginary.")
        rp = -b / (2 * a)
        ip = math.sqrt(-d) / (2 * a)
        print("The root1 is:", str(rp) + " + i" + str(ip))
        print("The root2 is:", str(rp) + " - i" + str(ip))

else:
    print("Not a quadratic equation.")
outputs
Enter the first coefficient: 1
Enter the second coefficient: -5
Enter the third coefficient: 6
The roots are real and distinct.
The root1 is: 3.0
The root2 is: 2.0
Enter the first coefficient: 1
Enter the second coefficient: -4
Enter the third coefficient: 4
The roots are real and equal.
The roots are 2.0 and 2.0
Enter the first coefficient: 1
Enter the second coefficient: 2
Enter the third coefficient: 5
The roots are imaginary.
The root1 is: -1.0 + i2.0
The root2 is: -1.0 - i2.0
