# Embedd
int a,b,c,d;
a = floor(distance);
b = (distance-a) * pow(10,3);

c = reversDigits (a);

d = reversDigits (b);

    while(c > 0) //do till num greater than  0
    {
        int mod = c % 10;  //split last digit from number
       char achar = '0' + mod;
       c=c/10;
LCD_data (achar);
}

LCD_data ('.');


    while(d > 0) //do till num greater than  0
    {
        int mod2 = d % 10;  //split last digit from number
        char bchar = '0' + mod2;
        d=d/10;
LCD_data (bchar);
    }
delayMs(500);

