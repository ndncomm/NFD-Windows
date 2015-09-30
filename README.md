# NFD-Windows
#1 Project goal: Run NFD on Windows

This implies: NFD dependencies should also work on Windows, including: ndn-cxx, Boost, sqlite3, CryptoPP.

#2 Current status

(1) Cygwin

 Successfully build NFD on Windows 7. Follow the steps to do it.
 We do not know if that works on other Windows versions or not. If you want to try, just try it.

(2) MinGW (compile on Windows)

 ndn-cxx is built as shared library.
 Attempting to start a tool (e.g. tlvdump) results in DLL initialization error.

(3) MinGW (MXE cross compile on Ubuntu)

 ndn-cxx is built as static library.
 Tools within ndn-cxx, such as ndncatchunks3 and tlvdump, works when connecting to remote NFD.
 NFD and ndn-tools have Boost link errors.
