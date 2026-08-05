import tkinter as tk


def fahrenheit_to_celsius():
    """Convert the entered temperature from Fahrenheit to Celsius

    and display the result in the label.
    """
    fahrenheit = ent_temperature.get()
    try:
        celsius = (float(fahrenheit) - 32) * 5 / 9
        lbl_result["text"] = f"{round(celsius, 2)} \N{DEGREE CELSIUS}"
    except ValueError:
        lbl_result["text"] = "Invalid input"


# Create the main window
window = tk.Tk()
window.title("Temperature Converter")
window.resizable(width=False, height=False)

# Create the frame for Fahrenheit input and label
frm_entry = tk.Frame(master=window)
ent_temperature = tk.Entry(master=frm_entry, width=10)
lbl_temp = tk.Label(master=frm_entry, text="\N{DEGREE FAHRENHEIT}")

# Arrange entry and label inside the frame
ent_temperature.grid(row=0, column=0, sticky="e")
lbl_temp.grid(row=0, column=1, sticky="w")

# Create conversion button and result label
btn_convert = tk.Button(
    master=window,
    text="\N{RIGHTWARDS BLACK ARROW}",
    command=fahrenheit_to_celsius,
)
lbl_result = tk.Label(master=window, text="\N{DEGREE CELSIUS}")

# Arrange frame, button, and result label in the main window
frm_entry.grid(row=0, column=0, padx=10)
btn_convert.grid(row=0, column=1, pady=10)
lbl_result.grid(row=0, column=2, padx=10)

# Run the application loop
window.mainloop()
