# MazeProject
Simple maze generator + solver based on backwards recursion with a user interface.


## Building the project:
This project uses CMAKE + conan for compilation and package management. Instructions for building the project are below; however, installation of CMAKE and conan are required before running below commands.


### First-Time Build:

Step 1: Clone the Repo
```bash
git clone https://github.com/JohnnyTRT/MazeProject.git
```

Step 2: Detect Machine OS & Compiler via conan
```bash
conan profile detect --force
```

Step 3: Install packages on device
```bash
conan install . -s --build_type=Release --build=missing
```

Step 4: Set Cmake Preset
```bash
cmake --preset conan-release
```

Step 5: Build
```bash
cmake --build --preset conan-release
```

Step 6: Acessing Build
Run final executable in bin/ folder 


### Building After the Initial Build:
After building the project once, you can build again after changes via step 5:
```bash
cmake --build --preset conan-release
```
