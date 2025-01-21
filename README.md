CodeAlpha Internship Task 2: Basic File Management

🚀 Excited to share my second task for the CodeAlpha Internship! This project involved creating a Basic File Management System in C++ to handle directories and files effortlessly.

💡 Key Features Implemented:

1️⃣ Create Directory: Create new folders dynamically.
2️⃣ Create File: Generate files with custom content.
3️⃣ View Directory Contents: Display files and folders in a directory.
4️⃣ View File Contents: Read and display file content.
5️⃣ Copy File: Duplicate files to a new location.
6️⃣ Move File: Relocate files efficiently.

🔧 Technologies Used:

C++: Core programming language.

Libraries:

<iostream>: Input/output operations.

<fstream>: File handling.

<direct.h> and <sys/stat.h>: Directory management.

<dirent.h>: Directory content retrieval.

<cstring>: Error handling.



📂 Functional Overview:

The program is menu-driven and provides a user-friendly interface to manage files and directories. This project not only strengthened my coding skills but also gave me hands-on experience in system-level file operations.

Here's a snippet from the program:

void createDirectory(const string& directoryName) {
    #ifdef _WIN32
        if (_mkdir(directoryName.c_str()) == 0) {
            cout << "Directory '" << directoryName << "' created successfully!\n";
        } else {
            cerr << "Error creating directory: " << directoryName << endl;
        }
    #else
        if (mkdir(directoryName.c_str(), 0777) == 0) {
            cout << "Directory '" << directoryName << "' created successfully!\n";
        } else {
            cerr << "Error creating directory: " << directoryName << endl;
        }
    #endif
}

This task has been an incredible learning experience, and I'm eager to tackle more challenges! 🎯

Would love to hear your thoughts or suggestions! 💬

#CodeAlpha #Internship #FileManagement #CPP

