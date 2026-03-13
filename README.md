# 🧩 OOP Basic Learning (C/C++)

**OOP Basic Learning (C/C++)** là repository được xây dựng trong quá trình học **lập trình hướng đối tượng (Object-Oriented Programming – OOP)** bằng **C/C++**, với mục tiêu lưu lại các **ví dụ minh họa**, **bài tập thực hành** và **kiến thức nền tảng** quan trọng.

Thông qua repository này, project tập trung hỗ trợ quá trình luyện tập:

* Tư duy lập trình hướng đối tượng
* Thiết kế `class` và `object`
* Tổ chức chương trình theo mô hình OOP
* Hiểu và áp dụng các nguyên lý nền tảng của OOP vào C/C++

Đây là một repository phù hợp cho sinh viên đang học các môn như:

* Lập trình C/C++
* Lập trình hướng đối tượng
* Cấu trúc dữ liệu và giải thuật cơ bản
* Kỹ thuật xây dựng chương trình nhiều module

Project được tổ chức theo hướng **đơn giản, rõ ràng, dễ hiểu và dễ thực hành**, giúp người học có thể theo dõi từng khái niệm OOP thông qua các ví dụ cụ thể.

---

# 📚 Nội dung đã học

Repository bao gồm các kiến thức OOP cơ bản và quan trọng trong C/C++ như sau:

## 1️⃣ Class và Object

Đây là khái niệm nền tảng đầu tiên của lập trình hướng đối tượng.

* `Class` dùng để mô tả khuôn mẫu của đối tượng
* `Object` là thực thể cụ thể được tạo ra từ class
* Class có thể chứa dữ liệu và các hàm thành viên

Ví dụ:

```cpp
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

## 2️⃣ Constructor

`Constructor` được sử dụng để **khởi tạo đối tượng** ngay khi object được tạo ra.

Thông qua constructor, người học có thể hiểu rõ hơn cách:

* khởi tạo dữ liệu ban đầu,
* giảm lặp code khi tạo object,
* và tổ chức class chuyên nghiệp hơn.

Ví dụ:

```cpp
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

## 3️⃣ Encapsulation (Đóng gói)

`Encapsulation` là nguyên lý giúp **bảo vệ dữ liệu** bên trong object bằng cách giới hạn quyền truy cập trực tiếp.

Trong C/C++, nguyên lý này thường được thực hiện bằng cách sử dụng:

* `private`
* `public`
* các hàm `setter/getter`

Ví dụ:

```cpp
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

## 4️⃣ Inheritance (Kế thừa)

`Inheritance` cho phép một class con kế thừa các thuộc tính và hành vi từ class cha.

Khái niệm này giúp:

* tái sử dụng mã nguồn,
* giảm trùng lặp,
* tổ chức chương trình theo cấu trúc hợp lý hơn.

Ví dụ:

```cpp
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

## 5️⃣ Polymorphism (Đa hình)

`Polymorphism` là khả năng một hành vi có thể được cài đặt theo nhiều cách khác nhau.

Trong C++, đa hình thường được thể hiện thông qua:

* `virtual function`
* ghi đè hàm ở class con

Ví dụ:

```cpp
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

Trong quá trình học và xây dựng repository này, các công cụ chính được sử dụng bao gồm:

* **C++**
* **GCC / g++ Compiler**
* **VS Code**

Đây là những công cụ phù hợp cho việc luyện tập lập trình hướng đối tượng trong môi trường học tập cơ bản.

---

# ▶️ Cách chạy chương trình

Bạn có thể biên dịch và chạy các file `.cpp` bằng trình biên dịch `g++`.

### 1️⃣ Compile

```bash
g++ main.cpp -o main
```

### 2️⃣ Run

Trên Linux / macOS:

```bash
./main
```

Trên Windows:

```bash
main.exe
```

---

# 📂 Cấu trúc repository

```text
oop-basic-learning
│
├── class_object.cpp
├── constructor.cpp
├── encapsulation.cpp
├── inheritance.cpp
└── polymorphism.cpp
```

| File | Mô tả |
| --- | --- |
| `class_object.cpp` | Ví dụ cơ bản về class và object |
| `constructor.cpp` | Minh họa constructor trong C/C++ |
| `encapsulation.cpp` | Minh họa nguyên lý đóng gói |
| `inheritance.cpp` | Minh họa cơ chế kế thừa |
| `polymorphism.cpp` | Minh họa cơ chế đa hình |

---

# 🎯 Mục tiêu của repository

* Lưu lại quá trình **học OOP** bằng **C/C++**
* Hiểu rõ các khái niệm quan trọng như **Class, Object, Constructor, Encapsulation, Inheritance, Polymorphism**
* Tạo tài liệu tham khảo cá nhân trong quá trình học lập trình hướng đối tượng
* Làm nền tảng cho các project lớn hơn sử dụng mô hình OOP
* Rèn luyện tư duy tổ chức chương trình theo hướng chuyên nghiệp và có cấu trúc

---

# 🧠 Giá trị học tập của project

Repository này có giá trị thực hành cao đối với sinh viên và người mới học OOP vì:

* giúp tiếp cận OOP theo từng khái niệm nhỏ,
* có ví dụ rõ ràng, dễ hiểu,
* thuận tiện cho việc tự học và ôn tập,
* tạo nền tảng cho việc học nâng cao như quản lý bộ nhớ, đa hình động, abstract class, interface và thiết kế phần mềm.

Đây là bước quan trọng để chuyển từ tư duy lập trình thủ tục sang tư duy lập trình hướng đối tượng.

---

# 👥 Đối tượng phù hợp

Repository này phù hợp với:

* Sinh viên đang học **C/C++**
* Người mới bắt đầu học **OOP**
* Người cần ví dụ cơ bản về **Class, Object, Inheritance, Polymorphism**
* Sinh viên muốn xây dựng nền tảng cho các project phần mềm lớn hơn

---

# 🚀 Hướng phát triển trong tương lai

Trong tương lai, repository có thể được mở rộng thêm với các nội dung như:

* Destructor
* Function Overloading
* Operator Overloading
* Abstract Class
* Interface
* Friend Function
* Static Member
* Project mini áp dụng OOP thực tế

Việc bổ sung các nội dung này sẽ giúp repository trở thành một tài liệu học tập đầy đủ hơn cho lập trình hướng đối tượng bằng C/C++.

---

# 👨‍💻 Tác giả

**Trần Gia Bảo** - **gibor06**

Sinh viên ngành **Công Nghệ Thông Tin** - **Trường Đại học Công Thương TP.HCM (HUIT)**

📍 TP.HCM, Việt Nam

# 📬 Liên hệ

📧 Email: [gibor06.dev@gmail.com](mailto:gibor06.dev@gmail.com)

🌐 Facebook: https://www.facebook.com/gibor06

---

# 📜 License

Repository này được sử dụng cho mục đích **học tập**, **thực hành** và **nghiên cứu**.
