# Stress-concentration-and-wellbore-breakout

Stress concentration around a wellbore occurs when there is a significant difference between the two horizontal stresses (Shmin and Shmax).

To better understand stress concentration around wellbore wall, we could calculate the Effective Hoop Stress (EHS) around the wellbore wall as a function of the azimuth or angle from the principle horizontal stress direction (Shmax or Shmin). For example, in the Python Notebook:[Stress_concentration.ipynb](/Stress_concentration.ipynb), the Effective Hoop Stress around wellbore wall is computed and ploted as a function of azimuth (angle from max horizontal stress direction, Shmax), so 0 and 180 degree refer to Shmax direction, and 90 degree refers to Shmin direction, as shown in the figure below. 

![image](https://github.com/user-attachments/assets/b5c6bb23-7567-4805-8ab3-9308efa98757)


We can see that the highest EHS happens at 90 degree which is at the Shmin direction. Physically, this means that there is a very high stress concentrated at the Shmin direction. With such a high Hoop Stress, wellbore wall could break and cause wellbore breakout. For example, if the rock strengh C0 is about 20000 psi, the breakout width will be about 60 degree (from 70 to 110 degree), but if the rock strength C0 is about 15000 psi, the breakout width will be increased to 80 degree (from 50 to 130 degree), as shown in the figure below.
![image](https://github.com/user-attachments/assets/b551d275-bd44-499b-99de-0ce5c75f4f44)


To limit the wellbore breakout width, we could also increase the mud weight. Because, as the mud weight increase, the EHS around the wellbore wall will decrease, as shown in the figure below. As MW increased from 4000 psi to 9000 psi, the breakout width decreased from 80 to 50 degree for a rock with strength C0 = 15000 psi.

![image](https://github.com/user-attachments/assets/17c56af3-b74e-46da-a32a-3a673a8fba3c)

Also, notice the EHS at 0 degree deceased from 0 to -5000 psi as MW increased. This will cause tensile fracture at the Shmax direction at the wellbore wall, a so-called drilling induced tensile fracture. 

Both the wellbore breakout and drilling induced tensile fracture can be visualized in the borehole image log, which is a very important data to analyze stress field and rock strength C0.

Drilling induced tensile fracture only occurs at near wellbore area at the Shmax direction, since as moving away from the wellbore wall, EHS retures to above 0 very quickly, as shown in the figure below.

![image](https://github.com/user-attachments/assets/f086470f-556c-4119-be4e-6f13ae1a9985)

Here the x axis is the normailized distance from the welbore wall. R=1 means at the wellbore wall. 

The equations for computing these calculations are captured in the uploaded Python Notebook: [Stress_concentration.ipynb](/Stress_concentration.ipynb).

Reference: Researvoir Geomechanics, Mark D. Zoback.




