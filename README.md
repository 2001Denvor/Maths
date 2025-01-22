import tkinter as tk
from tkinter import messagebox

#Question 01

def addition():
   user_input1=int(enter1.get())
   user_input2=int(enter2.get())
   if user_input1!=0 or user_input2!=0:
       result=[user_input1,user_input2]
       messagebox.showinfo("Output",f"Summation of two numbers is ={sum(result)} ")
   else:
       messagebox.showwarning("Output", "Please enter an one number at least up to 0.")


root=tk.Tk()
root.title("Addition two numbers.")
root.geometry("700x300")

label1=tk.Label(root, text="Enter first number:", font=("Arial",15))
label1.pack(pady=10)

enter1=tk.Entry(root)
enter1.pack(pady=5)

label2=tk.Label(root, text="Enter second number:", font=("Arial",15))
label2.pack(pady=10)

enter2=tk.Entry(root)
enter2.pack(pady=5)

button1=tk.Button(root, text="Submit", command=addition)
button1.pack(pady=12)

root.mainloop()


#Question 02

def check():
    user_enter=int(input.get())
    hence=user_enter%2
    if hence==0:
        messagebox.showinfo("Output",f"{user_enter} is even number.")
    else:
        messagebox.showinfo("Output",f"{user_enter} is odd number.")

root=tk.Tk()
root.title("Check the number is even or odd.")
root.geometry("400x200")

sticker=tk.Label(root, text="Enter Number : ", font=("Arial",15))
sticker.pack(pady=10)

input=tk.Entry(root)
input.pack(pady=5)

bullot=tk.Button(root, text="Submit", command=check)
bullot.pack(pady=12)

root.mainloop()



