# Midterm-

Button
from tkinter import *


class Window:
    def __init__(self, win):
        self.turn = 0
        self.button = Button(win, text="Color", bg='white', fg="black", command=self.colorChange)
        self.button.place(x=150, y=150)


    def colorChange(self):
        if self.turn == 0:
            self.turn += 1
            self.button.configure(bg='yellow', fg='red', activebackground='white', activeforeground='black')

        elif self.turn == 1:
            self.turn -= 1
            self.button.configure(bg='white', fg='black', activebackground='yellow', activeforeground='red')


tk = Tk()
window = Window(tk)
tk.geometry("300x350")
tk.title("Special Midterm In OOP")
tk.mainloop()


Fahrenheit to Celsius and Kelvin to Celsius


def main():
 class TemperatureConversion:
  def __init__(self, temp=1):
   self._temp = temp
 class CelsiusToFahrenheit(TemperatureConversion):
  def conversion(self):
   return (self._temp * 9) / 5 + 32
 class CelsiusToKelvin(TemperatureConversion):
  def conversion(self):
   return self._temp + 273.15

 tempInCelsius = float(input("Enter the temperature in Celsius: "))
 convert = CelsiusToKelvin(tempInCelsius)
 print(str(convert.conversion()) + " Kelvin")
 convert = CelsiusToFahrenheit(tempInCelsius)
 print(str(convert.conversion()) + " Fahrenheit")

temp = float(input("Enter temperature in Fahrenheit: "))
celsius = (temp - 32) * 5/9
print(f"{temp} in Fahrenheit is equal to {celsius} in Celsius")

temp = float(input("Enter temperature in Kelvin: "))
celsius = (temp - 273.15)
print(f"{temp} in Kelvin is equal to {celsius} in Celsius")

main()



