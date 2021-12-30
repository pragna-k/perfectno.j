# perfectno.j
import java.util.*;
public class perfectno
{
public static void main(String[] args)
{
Scanner knnc=new Scanner(System.in);
System.out.println("enter n value:");
int n=knnc.nextInt();
int i,j,c;
int sum=0;
for(i=1;i<n;i++)
{
c=0;
for(j=1;j<i;j++)
{
if (i%j==0)
{
c++;
}
}
if (c==1)
{
sum+=i;
}
}
if(sum==n)
{
System.out.println(n+" is a perfect number");
}
else
{
System.out.println(n+" is not a perfect number");
}
}
}
