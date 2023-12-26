### Hi there 👋

# Junzhe Yi
 ***
- 🔭 I’m currently a student in HUST, EIC.
- 📫 How to reach me: junzheyi.0719@gmail.com
- 😄 Pronouns: he/him
- 🌱 I’m currently learning AIGC
  
```python
import random
import time
import uuid

class Charles:
    def __init__(self, uuid: uuid.UUID) -> None:
        self.uuid = uuid
        self.gender = 'boy'
        self.pronouns = {'he', 'him', 'his'}
        self.girlfriend = 'Yuerou Liu'

    def career(self, year: int) -> str:
        current_year = time.localtime().tm_year
        if year < current_year:
            return f"In {year}, I was a student."
        elif year == current_year:
            return f"Now, I'm a wanderer in Huazhong University of Science and Technology!"
        else:
            return "Maybe in the future, I'm a ...! Well, who knows the future."

    def hobby(self) -> str:
        interests = [
            'Science Fiction', 'Machine Learning',
            'few-shot object detection', 'Running',
            'Badminton', 'English', "Mcdonald's",
            'Series', 'American blockbuster','AIGC'
        ]
        return random.choice(interests)

world = 'Universe'
uuid_ = uuid.uuid5(uuid.NAMESPACE_DNS, 'Charles Yee')

me = Charles(uuid_)

print(f"Hi! I'm Charles, a {me.gender}.")
print(f"I'm interested in {me.hobby()}.")
print(f"Feel free to contact me through yeecharles82@gmail.com / junzheyi.0719@gmail.com !")
