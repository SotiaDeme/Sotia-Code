The main concept with the Storm surge code is:
1. Get the dates from the wave climate file (wave climate file and water level file have the exact same dates)
2. Get the wave height values as they affect the overall depth
3. Get the water level values as they affect the overall depth
4. Get the fixed profile depth (will assume an average value from -0.2 meters until the depth of the breakwater)
5. Combine the fixed value, the wave height and the water level to obtain the overall depth per day (loop simulation)

Scenario 1: Assuming that the SS does not reach the shoreline (affects deep water only).
Deep water: Waves + WL + Actual Depth (Depth = WL + Profile depth)
At the breakwater: Waves + Actual depth (Actual depth = Depth at the breakwater) - Assessment of refraction and hbr
Behind the breakwater: Waves + Actual depth (Actual depth = Average profile depth) - Assessment of diffraction and hbr 

Scenario 2: Assuming that the SS does reach the shoreline.
Deep water: Waves + WL + Actual depth (Actual depth = WL + Profile depth)
At the breakwater: Waves + WL + Actual depth (Actual depth = WL + Depth at the breakwater) - Assessment of refraction and hbr
Behind the breakwater: Waves +WL + Actual depth (Actual depth = WL+ Average profile depth) - Assessment of diffraction and hbr
