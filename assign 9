#include <iostream>
#include <string>
using namespace std;

class Vehicle {
protected:
    string registrationNo;
    string brand;

public:
    Vehicle(string reg, string b) {
        registrationNo = reg;
        brand = b;
    }

    void displayCommon() const {
        cout << "Registration No: " << registrationNo << endl;
        cout << "Brand: " << brand << endl;
    }
};

class Car : public Vehicle {
    int seats;

public:
    Car(string reg, string b, int s) : Vehicle(reg, b) {
        seats = s;
    }

    void display() const {
        cout << "Car Details" << endl;
        displayCommon();
        cout << "Seating Capacity: " << seats << endl;
        cout << "------------------------" << endl;
    }
};

class Truck : public Vehicle {
    double loadCapacity;

public:
    Truck(string reg, string b, double load) : Vehicle(reg, b) {
        loadCapacity = load;
    }

    void display() const {
        cout << "Truck Details" << endl;
        displayCommon();
        cout << "Load Capacity: " << loadCapacity << " tons" << endl;
        cout << "------------------------" << endl;
    }
};

int main() {
    Car car("MH12AB1234", "Toyota", 5);
    Truck truck("MH14CD5678", "Tata", 12.5);

    car.display();
    truck.display();

    return 0;
}
