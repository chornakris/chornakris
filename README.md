from tkinter import *
def anime():
  if c.coords(f1)[0] < 400:
    c.move(f1, 1,0)
    c.move(f2,1, 0)
    c.move(f3,1, 0)
    c.move(f4,1,0)
    wind.after(15, anime)

wind = Tk()
wind.title('Ukraine')
c = Canvas(wind, width=600, height=300,bg="white")
c.pack()
f1=c.create_oval(100, 100, 200, 200, fill='#FFF933',outline='#335EFF', width=3)
f2=c.create_arc(120, 120, 180, 180, start=190, extent=160, style=ARC, outline='#335EFF', width=3)
f3=c.create_oval(125, 120, 140, 135, fill='#FFF933',outline='#335EFF', width=3)
f4=c.create_oval(160, 120, 175, 135, fill='#FFF933',outline='#335EFF', width=3)
anime()
wind.mainloop()
