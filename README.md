### Hi there 👋 I'm Junzhe Yi

<p><em>A bachelor student at <a href="https://www.hust.edu.cn">Huazhong University of Science and Technology</a>, majoring in Electronics and Information Engineering. 😊</br>
</em></p>

 ***
- 🔭 I’m currently a undergraduate student in HUST, EIC.
- 📫 How to reach me: junzheyi.0719@gmail.com
- 😄 Pronouns: he/him
- 🌱 I’m currently working on Anomaly Detection and AIGC.
  <img align="right" top='60' alt="GIF" src="https://raw.githubusercontent.com/devSouvik/devSouvik/master/gif3.gif" width="260"/>

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
            return f"Now, I'm a UG student in HuazhongUST!"
        else:
            return "Maybe in the future, I'm a ...!"

    def hobby(self) -> str:
        interests = [
            'Machine Learning','AIGC'
            'few-shot object detection',
            'Badminton', "Mcdonald's", 'Running',
        ]
        return random.choice(interests)

world = 'Universe'
uuid_ = uuid.uuid5(uuid.NAMESPACE_DNS, 'Charles Yee')

me = Charles(uuid_)

print(f"Hi! I'm Charles, a {me.gender}.")
print(f"I'm interested in {me.hobby()}.")
print(f"Feel free to contact me through yeecharles82@gmail.com / junzheyi.0719@gmail.com !")
