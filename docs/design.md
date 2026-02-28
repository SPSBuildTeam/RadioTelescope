
This section goes over the design considerations and choices made during the development of the physical radio telescope.

## Dish design:
to improve manufacturability the dish was segmented into even slices using the following considerations

angle of each slice:
$~ \theta = \frac{2π}{N} ~$  where N = number of slices of dish

arc length of slice: 
$~ S = \frac{2πr}{N} ~$ where $2r > \lambda$

focal length of dish:
 $~ f = \frac{r^2}{4d} ~$  where d is dish depth

Since we are trying to find the hyrogen line 
$f \approx 1420.4 ~ MHz$ giving $\lambda = \frac{c}{f} =  21.1 ~ cm$ 

this means $r > 10.55 ~ cm$
For easy construction we set r as 15 cm and N as 8, giving $S = 11.78 ~ cm$
