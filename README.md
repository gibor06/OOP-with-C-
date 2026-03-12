# 🧩 OOP Basic Learning (C/C++)

Repository này được tạo ra trong quá trình mình **học lập trình hướng đối tượng (OOP)** bằng **C/C++**.

Mục tiêu của repository là lưu lại:

* Ví dụ minh họa
* Bài tập thực hành
* Kiến thức nền tảng về OOP

Thông qua repository này, mình luyện tập:

* Tư duy lập trình hướng đối tượng
* Thiết kế class và object
* Xây dựng chương trình theo mô hình OOP

---

# 📚 Nội dung đã học

Các kiến thức OOP cơ bản trong repository bao gồm:

## 1. Class và Object

Ví dụ:

```cpp id="fl8h1h"
#include <iostream>
using namespace std;

class Student {
public:
    string name;
    int age;

    void display() {
        cout << name << " " << age << endl;
    }
};

int main() {
    Student s1;
    s1.name = "Bao";
    s1.age = 20;
    s1.display();
}
```

---

## 2. Constructor

Constructor được dùng để **khởi tạo đối tượng**.

```cpp id="9uhht8"
class Student {
public:
    string name;
    int age;

    Student(string n, int a){
        name = n;
        age = a;
    }
};
```

---

## 3. Encapsulation (Đóng gói)

Dùng `private` và `public` để bảo vệ dữ liệu.

```cpp id="ysks0n"
class Student {
private:
    int age;

public:
    void setAge(int a){
        age = a;
    }

    int getAge(){
        return age;
    }
};
```

---

## 4. Inheritance (Kế thừa)

```cpp id="i24ksc"
class Person {
public:
    string name;
};

class Student : public Person {
public:
    int studentID;
};
```

---

## 5. Polymorphism (Đa hình)

```cpp id="2x36ct"
class Animal {
public:
    virtual void sound(){
        cout << "Animal sound" << endl;
    }
};

class Dog : public Animal {
public:
    void sound(){
        cout << "Dog barks" << endl;
    }
};
```

---

# 🛠️ Công cụ sử dụng

Trong quá trình học mình sử dụng:

* **C++**
* **GCC / g++ Compiler**
* **VS Code**

---

# ▶️ Cách chạy chương trình

### 1. Compile

```bash id="jv7p6d"
g++ main.cpp -o main
```

### 2. Run

```bash id="bl4veq"
./main
```

Trên Windows:

```bash id="hb6i5j"
main.exe
```

---

# 📂 Cấu trúc repository

```id="3sjv4e"
oop-basic-learning
│
├── class_object.cpp
├── constructor.cpp
├── encapsulation.cpp
├── inheritance.cpp
└── polymorphism.cpp
```

---

# 🎯 Mục tiêu của repository

* Lưu lại quá trình **học OOP**
* Hiểu rõ các khái niệm **Class, Object, Inheritance, Polymorphism**
* Làm nền tảng cho các project lớn hơn

---

# 👨‍💻 Tác giả

**Trần Gia Bảo**

Sinh viên ngành **Công Nghệ Thông Tin**

Định hướng phát triển:

* Web Development
* Mobile Development
* Artificial Intelligence

---

# 📜 License

Repository này được sử dụng cho mục đích **học tập và nghiên cứu**.
