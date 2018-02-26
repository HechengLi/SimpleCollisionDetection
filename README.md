# SimpleCollisionDetection
Trying to write a simple collision detection which should be faster than bruteforce by paper, but not getting desired result.<br />
Currently it performs similar to bruteforce maybe 1~2ms faster in some cases.<br />
<br />
Current algorithm is to check if each item has collision in x or y axis, remember these items, then running a detailed check on each.<br />
This becomes extremely slow since when number of items is large enough there is almost always a collision in x or y, which makes this possibly slower than bruteforce.<br />
So I divided the items into 4 sections topleft, topright, bottomleft, bottomright and ran the algorithm on each section, this reduces the number of matches like when y collide but x are very different.<br />
Although the speed has increased dramatically, the algorithm itself from the beginning might not be very accurate.
