interface Shape {
    double area();
    double perimeter();
    void display();
}

class Circle implements Shape {
    double radius;
    Circle(double radius) { this.radius = radius; }
    public double area() { return Math.PI * radius * radius; }
    public double perimeter() { return 2 * Math.PI * radius; }
    public void display() {
        System.out.println("Shape: Circle");
        System.out.printf("  Radius    : %.2f\n", radius);
        System.out.printf("  Area      : %.2f\n", area());
        System.out.printf("  Perimeter : %.2f\n", perimeter());
    }
}

class Rectangle implements Shape {
    double length, width;
    Rectangle(double length, double width) { this.length = length; this.width = width; }
    public double area() { return length * width; }
    public double perimeter() { return 2 * (length + width); }
    public void display() {
        System.out.println("Shape: Rectangle");
        System.out.printf("  Length    : %.2f\n", length);
        System.out.printf("  Width     : %.2f\n", width);
        System.out.printf("  Area      : %.2f\n", area());
        System.out.printf("  Perimeter : %.2f\n", perimeter());
    }
}

class Triangle implements Shape {
    double a, b, c;
    Triangle(double a, double b, double c) { this.a = a; this.b = b; this.c = c; }
    public double area() {
        double s = (a + b + c) / 2;
        return Math.sqrt(s * (s - a) * (s - b) * (s - c));
    }
    public double perimeter() { return a + b + c; }
    public void display() {
        System.out.println("Shape: Triangle");
        System.out.printf("  Sides     : %.a2f, %.2f, %.2f\n", a, b, c);
        System.out.printf("  Area      : %.2f\n", area());
        System.out.printf("  Perimeter : %.2f\n", perimeter());
    }
}

public class ShapeDemo {
    public static void main(String[] args) {
        Shape[] shapes = { new Circle(7), new Rectangle(5, 8), new Triangle(3, 4, 5) };
        System.out.println("--- Shape Details ---");
        for (Shape s : shapes) { s.display(); System.out.println(); }
    }
}

