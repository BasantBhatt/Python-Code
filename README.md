# Class in Python

print("\t Welcome! Basant")


# Class Method
class Employee:
    company = "Camel"
    salary = 100
    location = "Kathmandu"

    def chasalary(self, sal):
        self.salary = sal

e = Employee()
print(e.salary)

e.chasalary(5000)       # Changes salary of: def chasalary class
print(e.salary)

print(Employee.salary)


# Class Method 2 (To change attributes of class)
class Employee:
    company = "Camel"
    salary = 100
    location = "Kathmandu"

    # def chasalary(self, sal):
    #    self.__class__.salary = sal    (Method 1)

    @classmethod                    # To change or add the attribute of classes
    def chasalary(cls, sal):
        cls.salary = sal

e = Employee()
print(e.salary)

e.chasalary(5000)      
print(e.salary)
print(Employee.salary)
