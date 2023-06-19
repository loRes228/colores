# Installation
* ### сURL
```bash
curl -o /usr/local/bin/colores https://raw.githubusercontent.com/loRes228/colores/main/colores && chmod +x /usr/local/bin/colores
```
<br>

* ### Wget
```bash
wget -O /usr/local/bin/colores https://raw.githubusercontent.com/loRes228/colores/main/colores && chmod +x /usr/local/bin/colores
```
<br>
<br>

# Usage examples
* ### Show help
```bash
colores -help
```
<br>

* ### Coloring text or background
```bash
echo -e "$(colores -fore 0 255 0)Green text using RGB color.$(colores -reset)"
echo -e "$(colores -back ff0000)Red background using HEX color.$(colores -reset)"
echo -e "$(colores -fore 200 -back 20)Purple text and blue background using ANSI color.$(colores -reset)"
```
<br>

![](https://i.imgur.com/2bPBh6w.png)
<br>
<br>

* ### Change the text style
```bash
echo -e "$(colores -style bold)Bold text$(colores -reset)"
echo -e "$(colores -style italic)Italic text$(colores -reset)"
echo -e "$(colores -style underline)Underline text$(colores -reset)"
echo -e "$(colores -style inverted)Inverted text$(colores -reset)"
echo -e "$(colores -style flashing)Flashing text$(colores -reset)"
echo -e "$(colores -style bold italic underline inverted flashing)All styles$(colores -reset)"
```
<br>

![](https://i.imgur.com/BD5npp5.gif)
<br>
<br>

* ### Using markers
```bash
echo -e "$(colores -mark success)Command executed successfully."
echo -e "$(colores -mark error)Command failed to execute."
echo -e "$(colores -mark warning)Proceed with caution."
echo -e "$(colores -mark info)Additional information provided."
echo -e "$(colores -mark question)Requesting user input."
echo -e "$(colores -mark question)Debugging information."
echo -e "$(colores -mark on)Command enabled."
echo -e "$(colores -mark off)Command disabled."
echo -e "$(colores -mark custom 'TEXT' 160 0 255)Custom marker using RGB color."
echo -e "$(colores -mark custom 'TEXT' 00C8FF)Custom marker using HEX color."
echo -e "$(colores -mark custom 'TEXT' 215)Custom marker using ANSI color."
```
<br>

![](https://i.imgur.com/YeJfpbl.png)
