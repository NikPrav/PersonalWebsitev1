# Graphs for B.ii
Runninng for different filter ratios, we get the bandwidth as follows
![[bandwidth_ratios.png]]
The most optimal solution here is to have a ratio of 0.2 for the least amount of stall cycles![[stall_cycles.png]]
Here, we can see that better the L2 ratio, better the bandwidth and lesser the amount of stall cycles.  Lesser switching wrt L2 buffer is ideal as it takes longer to switch, hence having a bigger L2 rather than L1 is favored, and helps in bandwidth and reducing compute cycles
# Graphs for B.iii
Changing the active buffer ratio, we get the following graphs![[bandwidth_active_buf.png]]![[stall_cycles_active_buf.png]]

Note: I was able to confirm using breakpoints that the values were being reflected, and were passed to the function correctly.