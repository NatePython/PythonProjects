# Can Improve so that I dont have to make a class for all pets and maybe create a database that has nodes for different animals
class Pet:
    def __init__(self, name,species,age,sex):
        self.name = str(name)
        self.species = str(species)
        self.age = str(age)
        self.sex = str(sex)

    def __str__(self):
        return f"{self.name} is a {self.species} dog and he or she is {self.age} old"

    def speak(self):
        print("IDK WHAT PET I AM")

# Specifying a Pet Type
class Dog(Pet):
    def __init__(self, name, species, age, sex):
        super().__init__(name,species,age, sex)

    def __str__(self):
        return f"{self.name} is a {self.species} {self.sex} dog and is {self.age} old"

    def speak(self):
        print(f"WOOF I AM {self.name} and I AM A {self.species} DOG")


# Specifying a Pet Type
class Cat(Pet):
    def __init__(self, name, species, age, sex):
        super().__init__(name, species, age, sex)

    def __str__(self):
        return f"{self.name} is a {self.species} {self.sex} cat and is {self.age} old"

    def speak(self):
        print(f"WOOF I AM {self.name} and I AM A {self.species} CAT")


        ## Im still leanrning
