# C++ FileShredder

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
