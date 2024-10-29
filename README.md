class Human:
    def __init__(self, name):
        self.name = name

    def introduce(self):
        print(f"Hello, my name is {self.name}")

class Nick(Human):
    def __init__(self, name, favorite_software):
        Human.__init__(self, name)
        self.favorite_software = favorite_software

    def code(self):
        print(f"I love create games in {self.favorite_software}")

nick = Nick("Nick", "Unreal Engine")
nick.introduce()
nick.code()
