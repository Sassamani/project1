#pragma once
#include<iostream>
using namespace std;
#include"Shape.h"
#include"Point.h"

class Cylinder : public Shape {
	friend ostream& operator<<(ostream&, const Cylinder&);
	friend istream& operator>>(istream&, Cylinder&);
private:
	Point P3;
	double radius;
	double height;
public:
	Cylinder();
	Cylinder(double,double, double, double);
	~Cylinder();
	double getX5()const;
	double getY5()const;
	double getradius()const;
	double getheight()const;

	int virtual print();
};
