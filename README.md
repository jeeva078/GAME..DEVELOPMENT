# EX 7 : THREE DIMENSIONAL TRANSFORMATIONS

## AIM :
 
 To implement the various transformations on three dimensional odjects using a c coding.

## EQUIPMENT REQUIRED:

●	Hardware: Personal Computer (PC)

●	Software: C Compiler

## ALGORITHM :


   Step 1 : Start.

   Step 2 : Draw an image with default parameters.

   Step 3 : Get the choice from user.

   Step 4 : Get the parameters for transformation.

   Step 5 : Perform the transformation.

   Step 6 : Display the output.

   Step 7 : Stop.

## Program :
~~~
#include<stdio.h> 
#include<conio.h> 
#include<graphics.h> 
#include<math.h> 
int maxx,maxy,midx,midy; 
void axis() 
{ 
getch(); 
cleardevice(); 
line(midx,0,midx,maxy); 
line(0,midy,maxx,midy); 
} 
void main() 
{ 
int gd,gm,x,y,z,o,x1,x2,y1,y2; 
detectgraph(&gd,&gm); 
initgraph(&gd,&gm,"c://turboc3//bgi");
setfillstyle(0,getmaxcolor()); 
maxx=getmaxx(); 
maxy=getmaxy(); 
midx=maxx/2; 
midy=maxy/2; 
axis(); 
bar3d(midx+50,midy-100,midx+60,midy-90,5,1); 
printf("Enter Translation Factor"); 
scanf("%d%d%d",&x,&y,&z); 
axis(); 
printf("after translation"); 
bar3d(midx+(x+50),midy-(y+100),midx+x+60,midy-(y+90),5,1); 
axis(); 
bar3d(midx+50,midy+100,midx+60,midy-90,5,1); 
printf("Enter Scaling Factor"); 
scanf("%d%d%d",&x,&y,&z); 
axis(); 
printf("After Scaling"); 
bar3d(midx+(x*50),midy-(y*100),midx+(x*60),midy-(y*90),5*z,1); 
axis(); 
bar3d(midx+50,midy-100,midx+60,midy-90,5,1); 
printf("Enter Rotating Angle"); 
scanf("%d",&o); 
x1=50*cos(o*3.14/180)-100*sin(o*3.14/180); 
y1=50*cos(o*3.14/180)+100*sin(o*3.14/180); 
x2=60*sin(o*3.14/180)-90*cos(o*3.14/180); 
y2=60*sin(o*3.14/180)+90*cos(o*3.14/180); 
axis(); 
printf("After Rotation about Z Axis"); 
bar3d(midx+x1,midy-y1,midx+x2,midy-y2,5,1); 
axis(); 
printf("After Rotation about X Axis"); 
bar3d(midx+50,midy-x1,midx+60,midy-x2,5,1); 
axis(); 
printf("After Rotation about Y Axis"); 
bar3d(midx+x1,midy-100,midx+x2,midy-90,5,1); 
getch(); 
closegraph(); 
}

Program to implement the various transformations on three dimensional odjects using a c coding.
DEVELOPED BY: MIDHUN S
REGISTER NUMBER: 212224230158
~~~
## Output :
![Screenshot 2025-05-08 113936](https://github.com/user-attachments/assets/13fbd135-6aac-4c79-9b9e-2b24869a1db4)
![Screenshot 2025-05-08 113948](https://github.com/user-attachments/assets/6460616c-9580-45fe-ac12-d8442b62e53f)
![Screenshot 2025-05-08 113959](https://github.com/user-attachments/assets/69847e67-ac48-4503-bb5a-e7850b7b7f50)
![Screenshot 2025-05-08 114017](https://github.com/user-attachments/assets/b2eede13-2da3-4e64-9602-f8244fa80a84)
![Screenshot 2025-05-08 114024](https://github.com/user-attachments/assets/9ea782f8-b025-4c01-a286-ba67b4825a1c)
![Screenshot 2025-05-08 114034](https://github.com/user-attachments/assets/35895457-2d28-4aaf-bb46-0cb47923b327)
![Screenshot 2025-05-08 114042](https://github.com/user-attachments/assets/d620e585-fa83-4bdc-8e2b-6bea81e94f6a)
![Screenshot 2025-05-08 114053](https://github.com/user-attachments/assets/16261176-5a6b-4f79-b6c1-858dd2e0c98a)


## Result :
Thus, the C program for performing three-dimensional transformations — including translation, scaling, and rotation about the X, Y, and Z axes — was successfully implemented and the output was verified through graphical representation.
