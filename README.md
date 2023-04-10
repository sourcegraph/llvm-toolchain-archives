# llvm-toolchain-archives

How to create an archive:
- On Windows, install [7-Zip](https://www.7-zip.org/download.html) (not strictly necessary, but makes unpacking simpler)
- Download an archive from the [LLVM releases page](https://github.com/llvm/llvm-project/releases/).
- Unpack the archive: right-click in the Downloads folder > 7-Zip > Extract to `LLVM-{version}-win64\`.
- In a Git Bash terminal, navigate to the Downloads folder an compress the archive.
  ```bash
  tar -cf LLVM-{version}-win64.tar --directory=. LLVM-{version}-win64
  xz --compress --threads 0 LLVM-{version}-win64.tar
  ```
  
Sourcegraph teammates can get access to a Windows machine
by selecting 'Windows Server' in GCP's Compute Engine.
