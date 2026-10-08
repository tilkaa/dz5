# dz5


#include <stdio.h>
#include <math.h>
#include <locale.h>

int main()
{
    double x, y, z, w;

    x = -2.235e-2;   
    y = 2.23;
    z = 15.221;

    double abs_xy = fabs(x - y);

    // кубический корень
    double part1 = cbrt(pow(x, 6) + pow(log(y), 2));

    // дробь 
    double chislitel = exp(abs_xy) * pow(abs_xy, x + y);
    double znamenatel = atan(x) + atan(z);
    double part2 = chislitel / znamenatel;

    w = part1 + part2;

    printf("x = %g\n", x);
    printf("y = %g\n", y);
    printf("z = %g\n", z);
    printf("\nw = %f\n", w);
    printf("w = %.3f\n", w);

    return 0;
}
