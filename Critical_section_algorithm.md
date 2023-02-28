software implementation of critical section

Peteresen's algorithm.

Algorithm 1
{
    do
    {
        while(turn!=i);
        Critical section
        turn=j
        Remainder section
    }while(1);
}

Algorithm 2
{
    do
    {
        flag[i]=true;
        while(flag[j]);
        Critical section
        flag[i]=false
        Remainding section
    }while(1);
}

Algorithm 3
{
    do
    {
        flag=[i]=true
        turn=j
        while(flag[j]&&turn==j);
        Critical section
        flag[i]=false
        Remainding section
    }while(1);
}

Bakery Algorithm
{
    do
    {
        choosing[i]=true;
        number[i]=max(number[0].....number[n-1]+1);
        chossing[i]=false;
        for(j=0;j<n;j++)
        {
            while(choosing[j]);
            while((number[j]!=0))&&(number[j],j)<(number[i],i);
        }
        Critical section
        number[i]=0;
        remainding section
    }while(1);
    
}