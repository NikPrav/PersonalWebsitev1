# Graph for 2A.i
![[graph.png]]
# Explanation for PE Mapping 
The filters are first filled and tiled in the filter_demand matrix normally, and the elements corresponding to the faulty PE is removed.

The elements are then mapped to a new tile, and then appended to the filter_demand matrix. The new tiles are filled in a specific order, which will help us to reduce the number of cycles:

![[SmartSelect_20240225_143232_OneNote.jpg]]
The numbers show the filling order. Every element along the blue line requires the given number of cycles. 

Since all elements correspond to the same partial sum, the ifmap_demand_matrix is the first row repeated according to the rows filled. Staggering the ifmap_demand rows is not required for the same reason. ==This leads to saving cycles due to the overhead introduced by skewing==
![[SmartSelect_20240225_145003_OneNote.jpg]]
Thus, instead of 54 cycles, the compute is finished within ==53 cycles==

W.r.t mapping efficiency, it is impossible for the array to achieve more than 84.375 percent
This is because we are given 27 input elements, and each tile has 8 PEs to be mapped. The absolute best case scenario is to use 4 tiles, which leads to ==27/32 = 84.375%==. (However, if i fill the last tile with one more element, i.e, use 28 elements instead of 27, i can get a better mapping efficiency on paper :D) 