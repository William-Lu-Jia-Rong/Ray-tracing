# Bill's Assignment2-part1

![graph here](/main/gears.png "gears")

This is a graph of the output from my code, I set up a founction for detecting whether the light hit the object or not. For the Sphere test, I used the equation provided during the course to do the calculation, |R(t)-C|^2-r^2=0 and |A+tD-C|^2-r^2=0. The rough process of the code is:
    double a=D*D;
    double b=2*D*(A-C);
    double c=(A-C)*(A-C)-r-*r;
    double delta=b*b-4*a*c;
    if(delta>0){
        double t1=(-b+sqrt(delta))/(2*a);
        double t2=(-b-sqrt(delta))/(2*a);
        if(t1<t2){
            t=t1;
        }
        else{
            t=t2;
        }
    }
    if(delta==0){
        t=-b/(2*a);
    }


For the triangle part, I also used the combine equation provided during the course which is: V1+ß(V2-V1)+gamma(V3-V1)=A+tD. The rough process of the code is: D(d0,d1,d2);
    V1(v10,v11,v12);
    V2(V20,v21,v22);
    V3(v30,v31,v32);
    A(a0,a1,a2);
    t=((a1-v11)*(v31-v11)-(a2-v12)*(v32-v12)-((v32-v12)*(v11-v21)-(v31-v11)*(v12-v22))*beta)/((v32-v12)*d1-(v31-v11)*d2)=g(beta);
    gamma=(d1*(a0-v10)-d0*(a1-v11)-(d1*(v10-v20)-d0*(v11-v21))*beta)/(d1*(v30-v10)-d0*(v31-v11))
    

These are all my main process.


