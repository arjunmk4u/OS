producer process

while(true)
{
    while(count==BUFFERSIZE);
    buffer[in]=next produced;
    in=(int)%BUFFERSIZE;
    count++;
}

Consumer process

while(true)
{
    while(count==0);
    next consumed=buffer[out]
    out=(out+1)%BUFFERSIZE;
    count--;
}