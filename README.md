# mkcomp
I'm tired of creating a new component structure every time for React.

Idea totally not stolen from [@joshwcomeau/new-component](https://github.com/joshwcomeau/new-component) ;)

Here's the folder/file breakdown:
* **Folder:** \<name-of-component\>

    - `index.js`: Contains the logic for the component

    - `styled.js`: Some sweet styling from `styled-components`

---

## Usage

1. The help command
    ```[bash]
    ➜ bash mkcomp --help
    mkcomp creates boilerplate code for a new React component and leverages styled-components.
    Usage: mkcomp [component-name-1] [component-name-2] ... [component-name-n]
    Type mkcomp -h or mkcomp --help to repeat this message.
    ```

2. Creating new components
    ```[bash]
    ➜ bash mkcomp Button Dropdown Sidebar Modal
    Project Directory: /home/codeabiswas/Developer/mkcomp
    Creating a components folder...
    Button has been successfully created!
    Dropdown has been successfully created!
    Sidebar has been successfully created!
    Modal has been successfully created!
    ```

---

## Installation

**Note:** This has only been tried and tested on Ubuntu. It has good chances of working with MacOS. Strong doubt on Windows (unless some WSL magic is involved but it hasn't been tested).

1. Clone or download this repo (unzip if downloaded).
2. Unless you have one already, create a root folder in your root directory called `bin/`.
```[bash]
cd ~
mkdir bin/
```
3. Add the absolute path of the `bin/` directory to your `.bashrc` (or `.bash_profile`, `.zshrc`, etc.) as shown below.
```[bash]
export PATH=$PATH:<absolute-path-of-bin/-directory>
```
4. Copy the `mkcomp` file to that folder
```[bash]
cp mkcomp ~/bin
```
5. Give `mkcomp` executable rights after entering the `bin/` folder
```[bash]
cd ~/bin
chmod +x mkcomp
```

---

## Contributors
* Andrei Biswas @codeabiswas
