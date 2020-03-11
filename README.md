# 3sumClosest

"""Algorithm:
step1:sort the array.(by sorting the array the smallest value can be point by one pointer and
the largest value can be point by another pointer).
step2:Iterate over each element of the array.
staep3:Initialise two pointers which will indicate the second element(S) of the array and 
the end element(E) of the array.
step5:compute the actual sum by summing up initial three numbers of the array
step4:while s less than e :
	do 1.compute the sum of array[i]+array[s]+array[e]
	2.now substract the target with the actualsum and the sum if actualsum<sum then
	 do:
	 actualsum=sum(we are doing this so that we can find the minimum value which is closest 
	 to target or else it can give you the maximum value)
	3.if sum less than target:
			increase s by one
	  else decrease e by one
	  (we know we need exactly closest value if sum less than target we have to
	   increment it so we can get sum greater than target else if the sum greater than target 
	   we have to decrement e because it is the largest value not the minimum closest value)
step 5:
	return actualsum
"""
