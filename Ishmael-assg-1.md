1.9: a)
solution:
Slowing clock rate reduce the power and dose not reduce the energy. 
Lets assume normal speed= x and execute time is twice normal speed= 2x 

![first equation](https://latex.codecogs.com/gif.latex?%5Cfrac%7B2x-x%7D%7B2x%7D%3D%5Cfrac%7B1%7D%7B2%7D*100%3D%2050%20percent)  
Energy saving

b) 

   Energy(old) = 1/2 * load capacitive* (V)^2
   
   Engery(new) = 1/2 * load capacitive* (1/2* V^2)^2 
   
   Engery(new)/Energy(old)= 1/4
   
C.1: a)
    
|Register|Source Instructor|Destination Instructor|
|--------|---------|---------|
|R_1|LD|DADDI|
|R_1|DADDI|SD|
|R_2|LD|DADDI|
|R_2|SD|DADDI|
|R_2|DADDI|DSUB|
|R_4|DSUB|BNEZ|

b)

||1|2|3|4|5|6|7|8|9|10|11|12|13|14|15|16|17|18|19|
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
|LD R_1, 0(R_2)|FT|DC|EI|MR|WRB|
|DADDI  R_1, R_1, #1| |FT|s|s|DC|EI|MR|WRB|
|SD 0(R_2), R_1|||||FT|s|s|DC|EI|MR|WRB|
|DADDI R_2, R_2, #4||||||||FT|DC|EI|MR|WRB|
|DSUB R_4,  R_3,  R_2|||||||||FT|s|s|DC|EI|MR|WRB|
|BNEZ R_4,Loop||||||||||||FT|s|s|DC|EI|MR|WRB|
|LD R_1,0(R_2)|||||||||||||||||FT|DC|



   
   
   

   
     
