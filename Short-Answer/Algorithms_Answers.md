#### Please add your answers to the ***Analysis of  Algorithms*** exercises here.

## Exercise I

a) Should be O(n) because as n increases at the same rate of the iterations


b) Should be O(n^2) because of the nested loop


c) Should be O(n) because there is 1 iteration for each n

## Exercise II


Plain english: We would do a binary search. Take n find the middle, if an egg get broken off of that floor, then make that n. Do this until we find the floors that are the divider and return the bottom floor (the highest floor where the egg doesn't break)

code:

def correctFloor(top = 30, bottom = 0,  floor = 18):
    mid = (top + bottom) // 2
    if mid > floor:
        egg == broke
    else:
        egg = not broke

    if bottom == top - 1:
        return bottom
    if egg == broke:
        return(correctFloor(mid, bottom, floor))
    else:
        return(correctFloor(top, mid, floor))

Wild guess but complexity would be O(n/2)
