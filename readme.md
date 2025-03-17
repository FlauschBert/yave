# GDextension Example
## git submodule
### run the first time
`git submodule update --init --recursive`
### update to new godot version
- make the changes in `.gitmodules`: change tag
- get and merge the changes: `git submodule update --remote --merge`
- add and commit the changes: `git add .gitmodules godot-cpp`
- `git commit -m "Update godot-cpp submodule"`