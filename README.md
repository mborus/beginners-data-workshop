# Humble Data Workshop

[![Humble Data Workshop](./media/humble-data-logo-transparent.png)](https://humbledata.org)

## ℹ️ If you would like to know more about this workshop, please [see our website](https://humbledata.org/).

---

Below are the set of instructions for different operating systems. Please go to the instructions for your specific operating system (Windows and Mac OS) and follow them to get started.

## Windows 10/11

* Download, then install git from https://git-scm.com/download/win
* Download, then install the latest python 3.12.4 from https://www.python.org/downloads/. Once it has downloaded, double-click on the file, and follow the instructions in the wizard.

You will likely need to run the following steps to use Python (see [this link](https://realpython.com/add-python-to-path/#how-to-add-python-to-path-on-windows)) for more details:
1. Find where Python was just installed. Go to the Start menu, then type Python. It will be called something like "Python 3.12 (64 bit)". Right click on this, and select "Open file location".
2. Go back into the "Programs" folder.
3. The folder containing Python will have the name of the Python version you just downloaded (e.g., Python 3.12). Copy the name of this folder (e.g., "C:\Users\joana\AppData\Roaming\Microsoft\Windows\Start Menu\Programs\Python 3.12"). [You _might_ need to change the name of this path so it doesn't contain any spaces - try steps 4 through 7, and if they don't work, try changing the final "Python 3.12" to "Python_3_12" and then repeat steps 4 through 7.] 

![](/media/windows-1.png)

4. Once you’ve located your Python executable, open the Start menu and search for the Edit the system environment variables entry, which opens up a System Properties window. In the Advanced tab, click on the button Environment Variables. There you’ll see User and System variables, which you’ll be able to edit.
5. In the section entitled User Variables, double-click on the entry that says Path. Another window will pop up showing a list of paths. Click the New button and paste the path to your Python executable there. Once that’s inserted, select your newly added path and click the Move Up button until it’s at the top.
6.  You may need to reboot your computer for the changes to take effect, but you should now be able to call python from the terminal. See if it works by opening a terminal window: do this by going to the Start menu, typing "cmd", and selecting "Command Prompt". 
7. Once you have this open, at the prompt (see the image below, where it says "C:\Users\joana>", type `py --version`. It should say something like `Python 3.12.4`. Don't worry if the numbers are not exactly the same.

**Note**: This section is only needed for setup. Next time you can skip them.

![](/media/windows-2.png)

* Next, in the terminal, do these steps:
1. Go to the desktop: copy and paste `cd Desktop` into the terminal and press enter to run this command. 
2. Run `git clone --depth 1 https://github.com/mborus/beginners-data-workshop` in the terminal. This will download all of the materials for this course.
3. Run `cd beginners-data-workshop` in the terminal.
4. Run `py -3.12 -m venv venv` in the terminal.
5. Run `.\venv\Scripts\activate` in the terminal.
6. Run `python -m pip install -r requirements.txt` in the terminal.
7. Run `jupyter-lab` in the terminal.
8. Wait for the browser to start with the notebook.

**Note**: Terminal steps 2, 4 and 6 are needed for setup. Next time you can skip them.

## Mac OS

1. Open Terminal on your Mac.
2. Go to https://brew.sh/ and follow the instructions. If you are unfamiliar with running from Terminal, you just need to paste `/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"` at the prompt in the Terminal, and press enter. This will install a program called Homebrew, which will allow us to install a bunch of stuff easily, including Python.
3. Run `brew install python@3.12` in the Terminal.
4. Run `brew install git` in the Terminal.
5. Run `git clone --depth 1 https://github.com/mborus/beginners-data-workshop` in the terminal. This will download all of the materials for this course.
6. Run `cd beginners-data-workshop` in the Terminal.
7. Run `python3.12 -m venv myenv` in the Terminal.
8. Run `source myenv/bin/activate` in the Terminal.
9. Run `jupyter-lab` in the Terminal. 
10. Wait for the browser to start with the notebook.

**Note**: All of the steps except steps 6, 8, 9 are only needed for setup, you will not need to repeat them next time.

## License

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License</a>.