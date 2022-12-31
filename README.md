## 🕯️ Steps to wish

* Clone this repo and install the requirements
    ```bash
    git clone https://github.com/hemantapkh/PyBirthdayWish.git && cd PyBirthdayWish && pip install -r requirements.txt
    ```
* Edit the ``arts/art.py`` file and add your texts and colors using color codes.

* Edit the ``config.py`` file to change the settings and make ``artFile = 'art'`` to use ``arts/art.py`` instead of ``example.py``.

* Run ``PyBirthdayWish.py`` with python3
    ```bash
    python3 PyBirthdayWish.py
    ```

* If everthing is working as intended, you can create an executable by using pyinstaller with the following command
    * On windows
        ```bash
        pyinstaller --noconfirm --onefile --console --icon "icon.ico" --no-embed-manifest --add-data "arts;arts/"  --add-data "config.py;." --add-data "HappyBirthday.mp3;." --add-data "PyBirthdayWish.py;."  "PyBirthdayWish.py"
        ```
    * On Unix based system
        ```bash
        pyinstaller --noconfirm --onefile --console --icon "icon.ico" --no-embed-manifest --add-data "arts:arts/"  --add-data "config.py:." --add-data "HappyBirthday.mp3:." --add-data "PyBirthdayWish.py:."  "PyBirthdayWish.py"
        ```

* Send the executable file (Inside dist folder) to your friend and wish them a pythonic happy birthday.
-----

Made with :heart: and Python.
