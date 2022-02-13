# Computer-graphics_6-semester
Laboratory work in Computer graphics 6 semester

# Installation
## Python
1. Execute `python --version` in the terminal and remember your Python version.
2. Go to the [site](https://www.lfd.uci.edu/~gohlke/pythonlibs/#pyopengl) and download the files:
    > PyOpenGL_accelerate‑3.15‑cpXXX‑cpXXX‑win32_amd64.whl

    > PyOpenGL‑3.1.5‑cpXXX‑cpXXX‑win_amd64.whl

    XXX - your Python version.
3. Execute `pip install PyOpenGL_accelerate‑3.15‑cpXXX‑cpXXX‑win32_amd64.whl && pip install PyOpenGL‑3.1.5‑cpXXX‑cpXXX‑win_amd64.whl`

    XXX - your Python version.
4. Try execute the sample `python XmasTreeSample/XmasTreeSample.py` in root of repository.

## C++ (MinGW)
1. Download **Freeglut 3.0.0 MinGW Package** [from](https://www.transmissionzero.co.uk/software/freeglut-devel).
2. Unpack from archive **freeglut/bin/x64** to **XmasTreeSample/C++/lib/freeglut**
3. Unpack from archive **freeglut/include/GL** to **XmasTreeSample/C++/include/freeglut**
4. Unpack from archive **freeglut/lib/x64/** to **XmasTreeSample/C++/include/freeglut**
5. Build:
    ```
    g++ -mwindows -D FREEGLUT_STATIC -D RELEASE -std=c++17 -Wall -Wextra -O3 -I XmasTreeSample/C++/include/freeglut -L XmasTreeSample/C++/lib/freeglut XmasTreeSample/C++/*.cpp -o C++.exe -lglu32 -lfreeglut_static -lopengl32 -lwinmm -lgdi32
    ```
6. Execute `C++.exe`