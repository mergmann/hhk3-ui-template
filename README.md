# hhk3-ui-template
A template for writing hollyhock-3 applications by using the system UI 

## How to Setup
1. Click **Use this template** in the GitHub interface and set up a repo
2. Clone your repository
3. Run `git submodule init --recursive` in the repo
4. Enter the devcontainer
5. `make compile_commands.json` or use the vscode task
6. Restart clangd (eg. via CRTL+SHIFT+P in vscode)

## How to build
```sh
# Build for OS 7002
make -j OS=7002

# Build for OS 2000
make -j OS=2000
```
Other OSes are currently not supported

## How to run
Copy `dist/UITemplate.hh3` to the root of the calculator when connected in usb storage mode and then select and run from the launcher.

## How to change the file name (recommended)
Open the Makefile and adjust this line to what you want:
```Makefile
APPNAME = UITemplate
```