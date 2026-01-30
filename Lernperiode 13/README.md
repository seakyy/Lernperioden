# [C++ FileShredder](https://github.com/seakyy/FileShredder)

Create a simple C++ Application which can permanently delete files. The windows "delete" function only deletes the reference to a file, however doesn't really delete the Contents of it. This application will delete the files content with overwriting it with zeros, ones and pseudo random data.

# 16.01.2026
- [ ] Collect information about Windows API.
- [ ] Implement Drag and Drop into the application.
- [ ] Implement file opening using "createfile".
- [ ] Error handling: Check if file is lcoked by another process


# 23.01.2026
- [ ] Implement File pointer management
- [ ] Add overwrite loop (core feature)
- [ ] cache-bypass with flushfilebuffer
- [ ] Better User safety (to prevent accidently deleting important files)

# 30.01.2026
- [ ] Add shreddering mechanism
- [ ] upgrade ui for better visibility
- [ ] should be able to handle multi thread
- [ ] Add docs and github pages

This project is finished _for now_, it runs on [GitHub Pages](https://seakyy.github.io/FileShredder/tutorial) with Docs.
