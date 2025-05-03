-- إنشاء قاعدة البيانات
CREATE DATABASE StudentDB;

-- استخدام قاعدة البيانات
USE StudentDB;

-- إنشاء جدول للطلاب
CREATE TABLE Students (
    student_id INT AUTO_INCREMENT PRIMARY KEY,
    first_name VARCHAR(50),
    last_name VARCHAR(50),
    email VARCHAR(100),
    dob DATE,
    total_classes INT,
    attended_classes INT
);

-- إدخال بعض البيانات
INSERT INTO Students (first_name, last_name, email, dob, total_classes, attended_classes)
VALUES
    ('Ahmed', 'Ali', 'ahmed@example.com', '2000-05-15', 30, 28),
    ('Sara', 'Mohamed', 'sara@example.com', '1999-07-22', 30, 30),
    ('Mona', 'Hassan', 'mona@example.com', '2001-03-10', 30, 25);

-- استعلام لعرض كل البيانات
SELECT * FROM Students;
