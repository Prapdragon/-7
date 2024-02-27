# -7
#1
income = float(input("กรุณาระบุรายได้ (บาท): "))

if income >= 15000 and income < 20000:
    credit_card_type = "บัตร Sliver"
elif income < 100000:
    credit_card_type = "บัตร Gold"
else:
    credit_card_type = "บัตร Platinum"

print(f"ตามรายได้ {income:.2f} บาท สามารถทำ{credit_card_type} ได้")
#2
score = int(input("ระบุคะแนน  "))

if score >= 80:
    grade = "A"
elif 70 <= score <= 79:
    grade = "B"
elif 60 <= score <= 69:
    grade = "C"
elif 50 <= score <= 59:
    grade = "D"
else:
    grade = "F"

print(f"คะแนน {score} ได้เกรด {grade}")
#3
correct_username = "admin"
correct_password = "Ad13n@23t"

username = input("Username: ")
password = input("Password: ")

if username == correct_username and password == correct_password:
    print("เข้าสู่ระบบสำเร็จ")
else:
    print("เข้าสู่ระบบไม่สำเร็จ กรุณาตรวจสอบ Username หรือ Password อีกครั้ง")
#4
weight_kg = float(input("น้ำหนัก (กิโลกรัม): "))
height_m = float(input("ส่วนสูง (เมตร): "))

bmi = weight_kg / (height_m ** 2)

print(f"BMI is: {bmi:.1f}")

if bmi < 18.5:
    print("Underweight")
elif 18.5 <= bmi < 25:
    print("Normal weight")
elif 25 <= bmi < 30:
    print("Overweight")
else:
    print("Obesity")
