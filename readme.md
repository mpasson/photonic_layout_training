# Photonic IC design tools installation guide

## Python

1. If you have ``python`` and ``pip`` installed, you can skip this section.

2. If not, install python from [python.org](https://www.python.org/downloads/). You can follow [this guide](https://realpython.com/installing-python/) for Windows. The suggested way is to follow the [How to install from the full installer](https://realpython.com/installing-python/#how-to-install-from-the-full-installer) part. Please remember to check the option to **add python to the PATH**.

3. Open a `Windows Powershell` and type ``python``. If you enter the python interactive python console everything is fine. If not, something is wrong and I suggest to redo the procedure. To exit the interactive windows just type ``quit()``.

4. It is advised to install a Python IDE. Suggested is [VSCode](https://code.visualstudio.com/), but popular options are [Spyder](https://www.spyder-ide.org/) or [PyCharm](https://www.jetbrains.com/pycharm/).

## Nazca Design

1. The installation of nazca and its requirements is managed by the package installer for Python ``pip`` program. In order to verify that you have it installed and working open a `Windows Powersheel` and run:

        pip --version

    If you see an output like this one:

        pip 23.3.1 from C:\Users\Marco.Passoni\AppData\Local\Programs\Python\Python311\Lib\site-packages\pip (python 3.11)

    everything is ok and you can move forward.

2. Download the requirements file [requirements.txt](./requirements.txt) and the [nazca installer](https://nazca-design.org/dist/nazca-0.5.13.zip) from [nazca-design.org](https://nazca-design.org/).

3. Put both files in the same folder, then open a `Windows Powershell` in the same folder.

4. Run the following commands to install the packages:

        pip install -r requirements.txt
        pip install nazca-0.5.13.zip

5. In order to verify the package is accessible enter the python interactive console by typing ``python``. Then run the following command:

        import nazca

    If you see this output:

        INFO: index.py: Index models version: 0.5.13

    everything is ok.

## Klayout

1. Go to the [Download](https://www.klayout.de/build.html) section of Klayout website.
2. Download the version compatible with your operating system and install it (for windows select 64bit installer).
3. Install it following the guided procedure.
