class Student:
def __init__(self, name, grade):
self.name = name
self.grade = grade


def display_info(self):
print(f"Όνομα: {self.name}, Βαθμός: {self.grade}")


student1 = Student("Γιάννης", 8.5)
student1.display_info()
