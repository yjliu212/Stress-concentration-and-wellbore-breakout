# Stress-concentration-and-wellbore-breakout

To better understand stress concentration around wellbore wall, we could calculate the Effective Hoop Stress (EHS) around the wellbore wall as a function of the azimuth or angle from the principle horizontal stress direction (Shmax or Shmin). For example, in the Python Notebook uploaded, the Effective Hoop Stress around wellbore wall is computed and ploted as a function of azimuth (angle from max horizontal stress direction, Shmax), so 0 and 180 degree refer to Shmax direction, as shown in the figure below. 

![image](https://github.com/user-attachments/assets/f5669773-9d1c-49f1-bf6e-d4f5fdafbd9a)

We can see that the highest EHS happens at 90 degree which is at the Shmin direction. Physically, this means that there is a very high stress concentrated at the Shmin direction. With such a high Hoop Stress, wellbore wall could break and cause wellbore breakout. For example, if the rock strengh C0 is about 20000 psi, the breakout width will be about 60 degree (from 70 to 110 degree), but if the rock strength C0 is about 15000 psi, the breakout width will be increased to 80 degree (from 50 to 130 degree), as shown in the figure below.

![image](https://github.com/user-attachments/assets/e81ea976-fe8a-4215-b223-8e7039c89b16)

To limit the wellbore breakout width, we could also increase the mud weight. Because, as the mud weight increase, the EHS around the wellbore wall will decrease, as shown in the figure below. As MW increase from 4000 psi to 9000 psi, the breakout width decreased from 80 to 50 degree for a rock strength C0 = 15000 psi type of rock.

![image](https://github.com/user-attachments/assets/9d7de49b-40c3-44aa-95b9-077fbfb745d3)

Also, notice the EHS at 0 and 180 degree deceased from 0 to -5000 psi as MW increase. This will cause tensile fracture at the Shmax direction at the wellbore wall, a so called drilling induced tensile fracture. 

Both the breakout and drilling induced tensile fracture can be visualized in the borehole image log, which is a very important data to analyze stress field and rock strength C0.

Drilling induced tensile fracture only occurs at near wellbore area at the Shmax direction, since as moving away from the wellbore wall, EHS retures to above 0 very quickly, as shown in the figure below.

![image](https://github.com/user-attachments/assets/246f6308-c73e-4cdb-8ca4-3e7c38063f66)

The equations for computing these calculations are captured in the Python Notebook Stress_concentration.ipynb.





