# hello
#我先照着代码打

#_*_coding:utf-8_*_
from tkinter import filedialog
import tkinter as tk
import jieba
import thinter.messagebox
import pickle
import wordcloud
import matpiotlib

#创建一个窗体
window = tk.Tk()#建立一个窗口
window.title("词云生成器")#命名窗体
window.geometry('450x300')#设置窗体大小
window.resizable(False, False)

#welcome image
canvas = tk.Canvas(window, height=300,width=450)
image_file = tk.PhotoImage(file='bg.gif')
image = canvas.create_image(0,0, anchor='nw',image=image_file)
canvas.pack(side=tk.LEFT)
