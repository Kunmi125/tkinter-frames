from tkinter import *

window = Tk()

# configure the main window to be resizeable
window.columnconfigure(0, weight = 1)
window.rowconfigure(0, weight = 1)
mf = Frame(window, borderwidth = 3, relief = "ridge")
mf.grid(padx = 50, pady = 50, sticky = "nsew")

# configure the main Frame
mf.columnconfigure(0, weight = 1)
mf.rowconfigure(0, weight = 2)
mf.columnconfigure(1, weight = 2)
f1 = Frame(mf, borderwidth = 3, relief = "ridge")
f1.grid(row = 0, column = 0, sticky = "nsew")
l1 = Label(f1, text = "Frame 1", )
l1.pack()


f2 = Frame(mf, borderwidth = 3, relief = "ridge")
f2.grid(row = 0, column = 1, sticky = "nsew")
l2 = Label(f2, text = "Frame 2", )
l2.pack()


window.mainloop()
