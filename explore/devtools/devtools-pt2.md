# Devtools Pt2

1. The bug is that num1 and num2 are both registered as strings, so it concatenates both of them, adding them as if they are strings. 
2. I would probably fix it by casting both of the nums into an int before adding, using parseInt(). 