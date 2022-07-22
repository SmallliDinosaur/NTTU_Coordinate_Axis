願促進臺東大學資訊發展，因此公布
<br>自標記檔案，如有使用<strong>請引用以下網址</strong>：
<br>
https://github.com/SmallliDinosaur/nttu_Coordinate_axis
```
from xml.etree import ElementTree as ET
tree=ET.parse('NTTU_MAP.xml')
root = tree.getroot()

for times in root.iter('Placemark'):
    name=times.find('name')
    point=times.find('Point')
    coordinates=point.find('coordinates')
    coordinates=str.strip(coordinates.text)
    count=-1
    for j in coordinates:
        count+=1
        if(j==','):
            b1=coordinates[:count]
            c1=coordinates[count+1:-2]
            break
    break
dictionary={}
dictionary.update({"w1":{"site":[b1,c1]}})
data.append(dictionary)
```
<br>
<br>
<br>
<br>
<br>
<br>⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⡖⠒⠒⠤⢄⠀⠀⠀
<br>⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢸⠁⠀⠀⠀⡼⠀⠀⠀⠀ ⠀
<br>⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢶⣲⡴⣗⣲⡦⢤⡏⠀⠀⠀⠀⠀
<br>⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣰⠋⠉⠉⠓⠛⠿⢷⣶⣦⠀⠀⠀
<br>⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢠⠇⠀⠀⠀⠀⠀⠀⠘⡇⠀⠀⠀⠀
<br>⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⡞⠀⠀⠀⠀⠀⠀⠀⢰⠇⠀⠀⠀⠀
<br>⠀⠀⠀⠀⠀⠀⠀⠀⡴⠊⠉⠳⡄⠀⢀⣀⣀⡀⠀⣸⠀⠀⠀⠀⠀
<br>⠀⠀⠀⠀⠀⠀⠀⢸⠃⠀⠰⠆⣿⡞⠉⠀⠀⠉⠲⡏⠀⠀⠀⠀⠀
<br>⠀⠀⠀⠀⠀⠀⠀⠈⢧⡀⣀⡴⠛⡇⠀⠈⠃⠀⠀⡗⠀⠀⠀⠀⠀
<br>⠀⠀⠀⠀⠀⠀⠀⠀⠀⣿⣱⠃⡴⠙⠢⠤⣀⠤⡾⠁⠀⠀⠀⠀⠀
<br>⠀⠀⠀⠀⠀⠀⠀⠀⢀⡇⣇⡼⠁⠀⠀⠀⠀⢰⠃⠀⠀⠀⠀⠀⠀
<br>⠀⠀⠀⠀⠀⠀⠀⠀⣸⢠⣉⣀⡴⠙⠀⠀⠀⣼⠀⠀⠀⠀⠀⠀⠀
<br>⠀⠀⠀⠀⠀⠀⠀⠀⡏⠀⠈⠁⠀⠀⠀⠀⢀⡇⠀⠀⠀⠀⠀⠀⠀
<br>⠀⠀⠀⠀⠀⠀⠀⢸⠃⠀⠀⠀⠀⠀⠀⠀⡼⠀⠀⠀⠀⠀⠀⠀⠀
<br>⠀⠀⠀⠀⠀⠀⠀⢸⠀⠀⠀⠀⠀⠀⠀⣰⠃⠀⠀⠀⠀⠀⠀⠀⠀
<br>⠀⠀⠀⠀⠀⣀⠤⠚⣶⡀⢠⠄⡰⠃⣠⣇⠀⠀⠀⠀⠀⠀⠀⠀⠀
<br>⠀⢀⣠⠔⣋⣷⣠⡞⠀⠉⠙⠛⠋⢩⡀⠈⠳⣄⠀⠀⠀⠀⠀⠀⠀
<br>⠀⡏⢴⠋⠁⠀⣸ 窩在留言區⣹⢦⣶⡛⠳⣄⠀⠀⠀⠀⠀
<br>⠀⠙⣌⠳⣄⠀⡇⠀⠀偷尿尿⠀⠀⡏⠀⠀⠈⠳⡌⣦⠀⠀⠀⠀
<br>⠀⠀⠈⢳⣈⣻⡇⠀⠀⠀⠀⠀⠀⢰⣇⣀⡠⠴⢊⡡⠋⠀⠀⠀⠀
<br>⠀⠀⠀⠀⠳⢿⡇⠀⠀⠀⠀⠀⠀⢸⣻⣶⡶⠊⠁⠀⠀⠀⠀⠀⠀
<br>⠀⠀⠀⠀⠀⢠⠟⠙⠓⠒⠒⠒⠒⢾⡛⠋⠁⠀⠀⠀⠀⠀⠀⠀⠀
<br>⠀⠀⠀⠀⣠⠏⠀⣸⠏⠉⠉⠳⣄⠀⠙⢆⠀⠀⠀⠀⠀⠀⠀⠀⠀
<br>⠀⠀⠀⡰⠃⠀⡴⠃⠀..⠀⠈⢦⡀⠈⠳⡄⠀⠀⠀⠀⠀⠀⠀
<br>⠀⠀⣸⠳⣤⠎⠀⠀⠀..⠀⠀⠀ ⠙⢄⡤⢯⡀⠀⠀⠀⠀⠀⠀
<br>⠀⠐⡇⠸⡅⠀⠀⠀⠀..⠀⠀⠀⠀⠀⠹⡆⢳⠀⠀⠀⠀⠀⠀
<br>⠀⠀⠹⡄⠹⡄⠀⠀⠀⠀..⠀⠀ ⠀⠀⣇⠸⡆⠀⠀⠀⠀⠀
<br>⠀⠀⠀⠹⡄⢳⡀⠀⠀ ..⠀⠀ ⠀⠀⢹⡀⣧⠀⠀⠀⠀⠀
<br>⠀⠀⠀⠀⢹⡤⠳⡄⠀⠀⠀..⠀⠀⠀⢀⣷⠚⣆⠀⠀⠀⠀
<br>⠀⠀⠀⡠⠊⠉⠉⢹⡀⠀..⠀⠀⠀⢸⡎⠉⠀⠙⢦⡀⠀
<br>⠀⠀⠾⠤⠤⠶⠒⠊⠀...⠀⠀ ⠀⠉⠙⠒⠲⠤⠽⠀
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<h3>🗺️校園地圖-手機板使用教學</h3>
-安卓：手機可直接點擊。<br>
-蘋果：建議複製- https://lihi1.com/fQBtx -至Safari。
<br>
![Imgur](https://imgur.com/gallery/apfxnZV)
<br>
<br>
<br>
<br>
表單範例：https://forms.gle/qV3Q6jdpAFWTqrj9A
<br>
來源檔案：
https://www.google.com/maps/d/edit?mid=1dcZM4HEzLQg6_afcW2bICPL1lAWxLK1y&usp=sharing
