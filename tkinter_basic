from tkinter import *
from datetime import datetime

def now_datetime():
    now = datetime.now()
    btn.config(text = now)
    btn.config(width = 25)
    
def side_change():
    if entry.get() != '':
#         btn.pack(side = entry.get())
        btn.pack(pady = entry.get())
    
window = Tk() # 창 생성

# 창 사이즈 설정 "가로x세로"
window.geometry("500x600")

# 창 title 설정
window.title("Time")

# 창 내용 폰트 설정
window.option_add("*Font","맑은고딕 20")

# 창 배경색 설정
window['bg']= '#c4c4c4'

# Entry 객체 생성  후 config로 속성 추가
entry = Entry(window)
entry.config(width = 10)
entry.pack()

# Button 객체 생성 후 config로 속성 추가
btn = Button(window)
btn.config(text = "지금 몇시에요?!")
btn.config(width = 15, height = 3)
# btn.config(command = now_datetime)
btn.config(command = side_change)
# 객체 배치 방법 3가지
btn.pack() # defualt 는 top, side = "left"식으로 위치 조절 가능
# btn.grid(row = 0, column = 0)
# btn.place(relx = 0.05, rely = 0.05) # x = 10, y = 15 이런식으로도 가능

window.mainloop() # 창 실행
