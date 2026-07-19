# OpenLi3DAR
A repository dedicated to open sourcing a way to convert a RPLiDAR C1 to a 3D LiDAR under $100

<img width="288" height="294" alt="image" src="https://github.com/user-attachments/assets/f59f3ba5-eb61-40d2-abf0-ba2925115169" />

## About The Project
This project started when I felt confined by the limits of a LiDAR that takes a 2D slice of its surroundings. When I used the RPLiDAR C1 on one of my other projects, [Weedl](https://github.com/sayithaStructs/Weedl), I started to understand the limitations with this 2D slice. Since Weedl was supposed to operate in open backyards, where there may be no fence or objects for the lasers to bounce back, oftentimes I would get incomplete maps. I didn't have the budget to afford the fancy 3D LiDARs out there, so I decided to see if I can modify my existing 2D LiDAR to get a 3D scan of Weedl's surroundings. 

While there were a couple resources online that have attempted the same thing (see acknowledgements), I wanted to make a complete guide as both resources had some holes and issues. Nonetheless, I definitely recommend checking those resources out.


## Bill Of Materials:
| Item         | Link | Price (as of 7/17/27) (USD) | Notes |
| ------------ | ---- | --------------------- | ----- |
| RPLiDAR C1   | [Amazon](https://www.amazon.com/WayPonDEV-RPLIDAR-C1-Avoidance-Navigation/dp/B0CMTXV5RC/ref=sr_1_1?adgrpid=187936274522&dib=eyJ2IjoiMSJ9.jnPLjqbbodzpJyq1oVvkcK7NIdOxOmzBbqJ4qItX7YyrrFoSk_prX17itXDso5aWm7KCu60bJ_9Qf1JL7aKnQ9n8DzcN_Hwp2bATC7_1_8xeyTUcMRWKDkKxGoAZdz4Ur5bvfql_bwcPH2oLbECd4j8yzqvXz3vfAw4Qv1LRcwgrU9oaLmz3oyxM0gshBPWQoWKwQL1JEegZGSvW8FG_xFLH9vm3kS8MMK4Ccg9X_O0._RRydRkpYwm5UYRXwetDLwarO3FSGMGUVt5LSB74tgA&dib_tag=se&hvadid=779662188950&hvdev=c&hvexpln=0&hvlocphy=9053131&hvnetw=g&hvocijid=16165029297544128341--&hvqmt=e&hvrand=16165029297544128341&hvtargid=kwd-2278706488518&hydadcr=19100_13454463_9741&keywords=rplidar+c1&mcid=70adc21eab9c37d18a29951d8510a3b6&qid=1784302388&sr=8-1)  | $74.99 | ------|
| N20 Motor    | [Amazon](https://www.amazon.com/Waveshare-All-Metal-Precision-Reduction-Connector/dp/B0CW1TCCTL/ref=sr_1_7?adgrpid=189241628569&dib=eyJ2IjoiMSJ9.injWYB3xXU30kLoB_z0HI2z1U5T7u0iZTN_DXQVUSQxYx56YyG30QxeDBZd4CKR70iRacdd9ebEye0GkEE8HXQu9TKDgIvdNwp1yqw6G6fB2hIk_yaQfixUWnREY0JmaEOgePj9KcEQJDdgYsCwCA1l-X7y4sZhREkyKlHbWLCi4CRD0eg65P6qpkRYur8-i-A_WTRIovIkVLw0Ifqce3zbjYrZP1MTi2ct69AcJrZ5d6rtUPOS2AH3zMW3w99U8Zwtuu2SG-D1sa1NqH-HEQdYcPDx6pWmIWBm1QN0jKaM.7dIoZVTmF9UJ5ghNruIJMC_qHgFYaSYByLAkl347cDg&dib_tag=se&hvadid=814208805561&hvdev=c&hvexpln=0&hvlocphy=9053131&hvnetw=g&hvocijid=2238680324220082900--&hvqmt=e&hvrand=2238680324220082900&hvtargid=kwd-984224244204&hydadcr=4126_13623928_18377&keywords=n20+gear+motor+with+encoder&mcid=b36959f0bad638458a5997e68771671e&qid=1784302286&sr=8-7)  | $10.99 | ------|
| Microcontroller/Driver    | [Amazon](https://www.amazon.com/dp/B014KMHSW6?lv=shuf&channelId=500&plpRedirect=mhFallback) | $6.99 | Using the L298N, though you can use any compatible driver |
| 3D Printed Parts    | [CAD Files] | ------ | Price depends on your means of printing it |
| Microcontroller     | ------ | Pre-owned | Will be using Raspberry Pi 5 |
| Total     | ------ | **$92.97** | ----- |

## Acknowledgements
[LIDAR PointCloud: 3D Mapping With Stepper Motor Control and Visualizer](https://www.instructables.com/LIDAR-PointCloud-3D-Mapping-With-Stepper-Motor-Con/)

[OpenLiDAR](https://github.com/patriciogonzalezvivo/openLiDAR)
