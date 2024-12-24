# Exp no:2 Fitting Poisson  distribution
Date:22-10-2024
# Aim : 

To fit poisson distribution for the arrival of objects per minute from the feeder

# Software required :  

Python and Visual component tool

# Theory:

The Poisson distribution is the discrete probability distribution of the number of events occurring in a given time period, given the average number of times the event occurs over that time period.

![image](https://user-images.githubusercontent.com/104613195/166248326-fd042076-8b0b-40c4-8b11-1d8e8fcb74db.png)

 Conditions for Poisson Distribution:

1. An event can occur any number of times during a time period.
2. Events occur independently. I
3. The rate of occurrence is constant.
4. The probability of an event occurring is proportional to the length of the time period. 
 
# Procedure :

![image](https://user-images.githubusercontent.com/104613195/166251988-d0c53205-6080-4f7b-ae4c-398178586637.png)

# Experiment :

![image](https://user-images.githubusercontent.com/103921593/230282876-f4a5afbf-cac1-4648-a1b0-c78840638a8e.png)

# Program :
DEVOLPED BY:NIRANJAN S
REF NO:24900209
import numpy as np

import math

import scipy.stats

L=[int(1) for i in input().split()]

N=len(L); M=max(L)

X=list();f=list()

for i in range (M+1):

    C=0

    for j in range(N):

        if L[j]==1:

           C=C+1

    f.append(c)

    X.append(1)

sf-np.sum(f)

p=list()

for i in range(M+1):

    p.append(f[i]/sf)

mean-np.inner(X,p)

p=list();E=list();xi-list()

print("X P(X=x) Obs. Fr Exp.Fr x1")

print("------------------------")

for x in range(M+1):

    p.append(math.exp(-mean)mean*x/math.factorial(x))

    E.append(p[x]sf)

    xi.append((f[x]-E[x])**2/E[x])

    print("%2.2f %2.3f %4.2f %3.2 %3.2f"%(x,p[x], f[x],E[x],xi[x]))

print("-------------------------------")

print("Calculated value of Chi square is %4.2f Xcal_ch12_sq)

cal_chi2_sq-np.sum(x1)

table_chi2-scipy.stats.chi2.ppf(1.01,df-M)

print("Table value of chi square at 1 level is %4.2f"Xtable_ch12)

if cal_chi2_sq<table_ch12:

    print("The given data can be fitted in poisson Distribution at 1X LOS")

else:

    print("The given data cannot be fitted in Poisson Distribution at 1% LOS")
 

# Output : 



# Results

The Poisson distribution is fitted for the objects arrived from feeder per minute and the data is tested using Chi-square test. 
 
