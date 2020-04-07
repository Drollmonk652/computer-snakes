/*  Percent Difference Function - (Requires the inclusion of the math.h library for fabs function)  */

double perdiff(double A, double B)
{
     return fabs(A-B)/((A+B)/2)*100;
}

/* end */

/*  Percent Error Function - (Requires the inclusion of the math.h library for fabs function) */

double pererr(double A, double B)
{
     return fabs(A-B)/A*100;
}

/* end */

/*  Column mean function    */

double col_mean(double x[NROWS][NCOLS], int col)
{
    int k;
    double sum=0;

    for(k=0;k<=NROWS-1;k++)
       sum+=x[k][col];

    return sum/NROWS;
}

/* end */


/*  Column standard deviation function		*/

double col_std_dev(double x[NROWS][NCOLS], int col)
{
    int k;
    double sumvar=0;
    double col_mean(double x[NROWS][NCOLS], int col);

    for(k=0;k<=NROWS-1;k++)
       sumvar+=((col_mean(x, col)-x[k][col])*(col_mean(x,col)-x[k][col]));

    return sqrt(sumvar/(NROWS-1));
}
