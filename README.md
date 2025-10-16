import tkinter as tk
from tkinter import font

# Create main window
root = tk.Tk()
root.title("DueDateDash 9A")
root.geometry("600x200")
root.configure(bg="#f5e6cc")  # soft brownish background

# Custom bubble font style (bold and rounded)
bubble_font = font.Font(family="Comic Sans MS", size=36, weight="bold")

# Create a label for the heading
heading = tk.Label(
    root,
    text="DueDateDash 9A",
    font=bubble_font,
    bg="#f5e6cc",
    fg="#a0522d",  # brownish color for text
    relief="raised",  # gives it a 3D bubble feel
    bd=8,  # thickness of bubble effect
    padx=20,
    pady=20
)

heading.pack(pady=40)

# Run the GUI
root.mainloop()
