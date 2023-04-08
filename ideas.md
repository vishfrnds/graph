# vflaot
inteligent version of float, which finds distribution of the values of each index of vector and then keeps more bits for dense part of distribution and less bit for sparse part of distribution

# seprate value and position vector in tranformers
keep less values for postion vector and more values for value vector.
attention of position vector can see value vector but attention of value vector can not see position vector

# compression of actual graph by lookup table
Since position and value vector are seprated, we can compress value vector by lookup table. For eg. all "THE" can point to single encoding of "THE" and all "AND" can point to single encoding of "AND".


# number of vectors to represent information should refelect amount of information
For starters we can use log(words) vectors to represent words.
But we can also have neural network that can predict amount of information in a current vector and then we can use that to decide how many vectors to keep in merged repersentation of the infomation. But all such value vector will have single postion vector.

We can also build a predictor to select 20% of vector randomly and then try to predict remaining, if we can predict it with high accuracy we can ignore them, else keep them.
