### Hi there 👋 I'm Junzhe Yi

<p><em>Undergraduate at <a href="https://www.hust.edu.cn">Huazhong University of Science and Technology</a>, majoring in Electronics and Information Engineering. 😊</br>
</em></p>
<p><em>Incoming Master student supervised by Prof. <a href="https://xwcv.github.io/">Xinggang Wang</a>.</em></p>




```python
import random
import time
import uuid

class Charles:
    def __init__(self, uuid: uuid.UUID) -> None:
        self.uuid = uuid
        self.pronouns = {'he', 'him', 'his'}

    def career(self, year: int) -> str:
        current_year = time.localtime().tm_year
        if year < current_year:
            return f"In {year}, I was a student."
        elif year == current_year:
            return f"Daydream"
        else:
            return "Till ···"

    def hobby(self) -> str:
        interests = [
            'Physical AI', 'VLA', 'Embodied Intelligence'
        ]
        return random.choice(interests)

world = 'Universe'
uuid_ = uuid.uuid5(uuid.NAMESPACE_DNS, 'Charles Yee')

me = Charles(uuid_)

print(f"Hi! I'm Charles, interested in {me.hobby()}.")
print(f"Feel free to contact me through charlesyeeme@gmail.com !")
