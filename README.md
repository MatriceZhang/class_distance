class_distance
==============

//
//  main.cpp
//  chapter 6
//
//  Created by zhangshiyu on 11/13/14.
//  Copyright (c) 2014 ZSY. All rights reserved.
//

#include <iostream>
using namespace std;

class Distance
{
private:
    int feet;
    float inches;
public:
    void setdist(int ft,float in)  //set Distance to args
    {feet=ft;inches=in;}
    void getdist()  //get lenghth from users
    {
        cout<<"\nEnter feet: "; cin>>feet;
        cout<<"Enter inches: ";cin>>inches;
    }
    
    void showdist()   //display distance
    {cout<<feet<<"\'-'"<<inches<<'\"';}
};

int main()
{
    Distance dist1,dist2;
    dist1.setdist(11, 6.25);  //define two length
    dist2.getdist();  //get dist2 form users
    
    
           //display length
    cout<<"\ndist1=";dist1.showdist();
    cout<<"\ndist2=";dist2.showdist();
    cout<<endl;
    return 0;
}
