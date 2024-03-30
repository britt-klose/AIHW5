# AIHW5: Optimum Design of an I-beam

# Description
The general optimization goal for this I-beam problem is to minimize F=[f1,f2]T where the cross section area (f1) and the static deflection (f2) of the I-beam are defined as:
f1(x)= 2*x2*x4+x3*(x1-2*x4)
f2(x)= 60000 / x3*(x1-2*x4)^3 + 2*x2*x4 *(4*x4^2 + 3*x1 *(x1-2*x4))
The two objectives are conflicting in nature since minimization of f1 will result in maximization of f2 and vice versa.

#Results
I outputed a graph for each function each showing the best and average fitness values in each generation. The results can be seen in the colab file included in the respository. 
I was surprised to not see much variation between all the graphs. Even when I manipulated the values for a and b -where [a,b] is the weight vector in F = a*f1 + b*f2 and adjusting them alters the level of importance associated with each function- there wasn't much difference between the graphs, as can be seen in the code file. Perhaps if I adjusted the axises there would be a more visual change. However when I played around with the values of Pc(crossover probability) and Pm(mutation probability) I did see more activity and more variation across the graphs. Visuals can be viewed in the AIHW5pics folder. The image files of the resulting graphs are named accordingly with the values of Pc and Pm. Based on the results it appears that more activity occurred from increasing the mutation probability and wasn't as affected by a change in the probability of crossover. Mutation probability lead to more drastic changes (up and down) in the average fitness level across the generations.  


