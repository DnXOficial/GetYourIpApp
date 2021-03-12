# GetYourIpApp

É um simples aplicativo, onde se objetivo é facilitar o acesso ao seu Endereço IPV4 (IP [IPv4]).

## Usage

```python
import sys
import socket

hostname = socket.gethostname()
ip_address = socket.gethostbyname(hostname)

try:
    import Tkinter as tk
except ImportError:
    import tkinter as tk

try:
    import ttk

    py3 = False
except ImportError:
    import tkinter.ttk as ttk

    py3 = True


def ipgetadress():
    pass


class Toplevel1:
    def __init__(self):
        '''This class configures and populates the toplevel window.
           top is the toplevel containing window.'''
        _bgcolor = '#d9d9d9'  # X11 color: 'gray85'
        _fgcolor = '#000000'  # X11 color: 'black'
        _compcolor = '#d9d9d9'  # X11 color: 'gray85'
        _ana1color = '#d9d9d9'  # X11 color: 'gray85'
        _ana2color = '#ececec'  # Closest X11 color: 'gray92'

        self.root = tk.Tk()
        self.root.geometry("600x450+323+136")
        self.root.minsize(120, 1)
        self.root.maxsize(1364, 749)
        self.root.resizable(1, 1)
        self.root.title("Login Area")
        self.root.configure(background="#6c00c6")

        self.Frame1 = tk.Frame(self.root)
        self.Frame1.place(relx=0.067, rely=0.067, relheight=0.856
                          , relwidth=0.875)
        self.Frame1.configure(relief='flat')
        self.Frame1.configure(borderwidth="2")
        self.Frame1.configure(background="#151515")

        self.Entry1 = tk.Entry(self.Frame1)
        self.Entry1.place(relx=0.305, rely=0.364, height=30, relwidth=0.389)
        self.Entry1.configure(background="white")
        self.Entry1.configure(disabledforeground="#a3a3a3")
        self.Entry1.configure(font="TkFixedFont")
        self.Entry1.configure(foreground="#000000")
        self.Entry1.configure(insertbackground="black")

        self.Entry1_1 = tk.Entry(self.Frame1, show='*')
        self.Entry1_1.place(relx=0.305, rely=0.545, height=30, relwidth=0.389)
        self.Entry1_1.configure(background="white")
        self.Entry1_1.configure(disabledforeground="#a3a3a3")
        self.Entry1_1.configure(font="TkFixedFont")
        self.Entry1_1.configure(foreground="#000000")
        self.Entry1_1.configure(highlightbackground="#d9d9d9")
        self.Entry1_1.configure(highlightcolor="black")
        self.Entry1_1.configure(insertbackground="black")
        self.Entry1_1.configure(selectbackground="blue")
        self.Entry1_1.configure(selectforeground="white")

        self.Label1 = tk.Label(self.Frame1)
        self.Label1.place(relx=0.267, rely=0.0, height=61, width=244)
        self.Label1.configure(activeforeground="#000000")
        self.Label1.configure(background="#151515")
        self.Label1.configure(disabledforeground="#a3a3a3")
        self.Label1.configure(font="-family {Sylfaen} -size 24 -weight bold -slant italic")
        self.Label1.configure(foreground="#f8f8f8")
        self.Label1.configure(text='''Get Your IP''')

        self.Label1_1_1 = tk.Label(self.Frame1)
        self.Label1_1_1.place(relx=0.286, rely=0.286, height=31, width=94)
        self.Label1_1_1.configure(activebackground="#f9f9f9")
        self.Label1_1_1.configure(activeforeground="#000000")
        self.Label1_1_1.configure(background="#151515")
        self.Label1_1_1.configure(disabledforeground="#a3a3a3")
        self.Label1_1_1.configure(font="-family {Segoe UI Symbol} -size 11")
        self.Label1_1_1.configure(foreground="#ffffff")
        self.Label1_1_1.configure(highlightbackground="#d9d9d9")
        self.Label1_1_1.configure(highlightcolor="#000000")
        self.Label1_1_1.configure(text='''Username''')

        self.Label1_1_1_1 = tk.Label(self.Frame1)
        self.Label1_1_1_1.place(relx=0.286, rely=0.468, height=31, width=94)
        self.Label1_1_1_1.configure(activebackground="#f9f9f9")
        self.Label1_1_1_1.configure(activeforeground="#000000")
        self.Label1_1_1_1.configure(background="#151515")
        self.Label1_1_1_1.configure(disabledforeground="#a3a3a3")
        self.Label1_1_1_1.configure(font="-family {Segoe UI Symbol} -size 11")
        self.Label1_1_1_1.configure(foreground="#ffffff")
        self.Label1_1_1_1.configure(highlightbackground="#d9d9d9")
        self.Label1_1_1_1.configure(highlightcolor="#000000")
        self.Label1_1_1_1.configure(text='''Password''')

        self.Label1_1_1_2 = tk.Label(self.Frame1)
        self.Label1_1_1_2.place(relx=0.076, rely=0.909, height=31, width=444)
        self.Label1_1_1_2.configure(activebackground="#6b6b6b")
        self.Label1_1_1_2.configure(activeforeground="white")
        self.Label1_1_1_2.configure(activeforeground="#000000")
        self.Label1_1_1_2.configure(background="#151515")
        self.Label1_1_1_2.configure(disabledforeground="#a3a3a3")
        self.Label1_1_1_2.configure(font="-family {Segoe UI Symbol} -size 14")
        self.Label1_1_1_2.configure(foreground="#1e1e1e")
        self.Label1_1_1_2.configure(highlightbackground="#d9d9d9")
        self.Label1_1_1_2.configure(highlightcolor="#000000")
        self.Label1_1_1_2.configure(text='''https://discord.gg/q4eBCDqxBa''')

        self.Button1 = tk.Button(self.Frame1, command=self.loginVerificationSystem)
        self.Button1.place(relx=0.381, rely=0.675, height=34, width=117)
        self.Button1.configure(activebackground="#ececec")
        self.Button1.configure(activeforeground="#000000")
        self.Button1.configure(background="#6c00c6")
        self.Button1.configure(disabledforeground="#a3a3a3")
        self.Button1.configure(font="-family {Segoe UI Historic} -size 12")
        self.Button1.configure(foreground="#ffffff")
        self.Button1.configure(highlightbackground="#d9d9d9")
        self.Button1.configure(highlightcolor="black")
        self.Button1.configure(pady="0")
        self.Button1.configure(relief="flat")
        self.Button1.configure(text='''Login''')
        self.root.mainloop()

    def loginVerificationSystem(self):
        with open('users.txt', 'r') as users:
            userlist = users.readlines()

        with open('passwords.txt', 'r') as passwords:
            pwlist = passwords.readlines()

        userlist = list(map(lambda x: x.replace('/n', ''), userlist))
        pwlist = list(map(lambda x: x.replace('/n', ''), pwlist))

        userlog = self.Entry1.get()
        passwordlog = self.Entry1_1.get()

        for i in range(len(userlist)):
            if userlog == userlist[i] and passwordlog == pwlist[i]:
                print('User Login Sucefully')
                self.root.destroy()

                try:
                    import Tkinter as tk
                except ImportError:
                    import tkinter as tk

                try:
                    import ttk
                    py3 = False
                except ImportError:
                    import tkinter.ttk as ttk
                    py3 = True

                class Toplevel2:
                    def __init__(self, top=None):
                        _bgcolor = '#d9d9d9'
                        _fgcolor = '#000000'
                        _compcolor = '#d9d9d9'
                        _ana1color = '#d9d9d9'
                        _ana2color = '#ececec'

                        top = tk.Tk()
                        top.geometry("600x450+391+206")
                        top.minsize(120, 1)
                        top.maxsize(1364, 749)
                        top.resizable(1, 1)
                        top.title("GetIP")
                        top.configure(background="#0f0f0f")

                        self.menubar = tk.Menu(top, font="TkMenuFont", bg=_bgcolor, fg=_fgcolor)
                        top.configure(menu=self.menubar)

                        self.Button1 = tk.Button(top, command=self.helloworld)
                        self.Button1.place(relx=0.367, rely=0.533, height=34, width=147)
                        self.Button1.configure(activebackground="#ececec")
                        self.Button1.configure(activeforeground="#000000")
                        self.Button1.configure(background="#d20005")
                        self.Button1.configure(disabledforeground="#a3a3a3")
                        self.Button1.configure(font="-family {THUNDER JAGGER} -size 18 -slant italic")
                        self.Button1.configure(foreground="#000000")
                        self.Button1.configure(highlightbackground="#d9d9d9")
                        self.Button1.configure(highlightcolor="black")
                        self.Button1.configure(pady="0")
                        self.Button1.configure(relief="flat")
                        self.Button1.configure(text='''Get IP''')

                        self.LabelR = tk.Label(top)
                        self.LabelR.place(relx=0.317, rely=0.467, height=21, width=204)
                        self.LabelR.configure(background="#ffffff")
                        self.LabelR.configure(disabledforeground="#a3a3a3")
                        self.LabelR.configure(font="-family {Yu Gothic} -size 9 -weight bold -slant italic")
                        self.LabelR.configure(foreground="#000000")
                        self.LabelR.configure(text='''Waiting Push The Button''')
                        top.mainloop()

                    def helloworld(self):
                        self.LabelR['text'] = ip_address

                Toplevel2()

            else:
                print('Error')
                self.root.destroy()


Toplevel1()

```

## License
Este Progama Foi Feito Para Pegar Seu IP, Nao Nos Responsabilizamos Caso Alguem Use Para Outros Propositos
