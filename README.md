The main concept with the Storm surge code is:
1. Get the dates from the wave climate file (wave climate file and water level file have the exact same dates)
2. Get the wave height values as they affect the overall depth
3. Get the water level values as they affect the overall depth
4. Get the fixed profile depth (will assume an average value from -0.2 meters until the depth of the breakwater)
5. Combine the fixed value, the wave height and the water level to obtain the overall depth per day (loop simulation)
