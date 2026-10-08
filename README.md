# Steps-to-Create-Two-Separate-Files-in-D-Directory-and-Compare-the-Text-Content

> **Disclaimer:** This project has been prepared for academic and personal purposes only, and represents the sole individual work of the author named above. No part of this project may be copied, reproduced, quoted, distributed, or used in any form — in whole or in part — without prior written permission from the author.

# Table of Contents

- [Introduction](#introduction)
- [Steps](#steps)
- [Commands Required](#commands-required)
- [References](#references)
- [Contact](#contact)

# Introduction
In system administration, managing files using command-line tools is essential. This project demonstrates how to create two separate files in a Linux environment (Kali Linux), write content into each, and compare their contents using built-in system commands (`diff` and `sdiff`). This task helps administrators detect changes or inconsistencies between text files, configuration files, or code files.

# Steps
### Step 1: Create the Project Directory and Navigate to It
In this step, we use the `mkdir` command to create a new directory for the project, and the `cd` command to navigate into it.

```bash
mkdir -p ~/Projects/Mohammed-FileCompare
cd ~/Projects/Mohammed-FileCompare
```

![createprojectfolder](ImagesProject/create-project-folder.png)

### Step 2: Create the Files and Write Content
In this step, we use the `echo` command to create two text files (`file1.txt` and `file2.txt`) and write content into them. The `>` operator is used to create/overwrite the file, while the `>>` operator is used to append additional text. We also include the author's copyright information in both files.

```bash
echo "Author: Mohammed Abdulrahman Alalyani (malredfan)" > file1.txt
echo "Hello, this is file one." >> file1.txt

echo "Author: Mohammed Abdulrahman Alalyani (malredfan)" > file2.txt
echo "Hello, this is file two with some changes." >> file2.txt
```

![create-files-with-copyright](ImagesProject/create-files-with-copyright.png)

### Step 3: Compare the Files Using `diff`
In this step, we use the `diff` command to compare the two files line by line. This command displays the differences between `file1.txt` and `file2.txt`.

```bash
diff file1.txt file2.txt
```

![diff-output](ImagesProject/diff-output.png)

### Step 4: Compare the Files Side-by-Side Using `sdiff`
In this step, we use the `sdiff` command to compare the two files side-by-side. This provides a clearer visual representation of the differences, showing both files in parallel columns.

```bash
sdiff file1.txt file2.txt
```

![sdiff-output](ImagesProject/sdiff-output.png)

# Commands Required
| Command | Description |
|---------|-------------|
| `mkdir` | Creates a new directory. |
| `cd`    | Changes the current directory. |
| `echo`  | Writes text to a file (`>` overwrites, `>>` appends). |
| `diff`  | Compares two files line by line. |
| `sdiff` | Compares two files side-by-side. |
| `cat`   | Displays the content of a file. |

# References

- GNU Operating System. (n.d.). *Diffutils - GNU Project*. Free Software Foundation. Retrieved from https://www.gnu.org/software/diffutils/
- Git. (n.d.). *Git Documentation*. Retrieved from https://git-scm.com/doc
- GitHub. (n.d.). *GitHub Docs*. Retrieved from https://docs.github.com/
- Linux man pages. (n.d.). *diff(1) - Linux manual page*. Retrieved from https://man7.org/linux/man-pages/man1/diff.1.html
- Linux man pages. (n.d.). *sdiff(1) - Linux manual page*. Retrieved from https://man7.org/linux/man-pages/man1/sdiff.1.html
- Microsoft Documentation: FC Command (Original Assignment Reference).
- Personal practice on Kali Linux (CCY253 - Systems Administration).

# Contact
For questions, feedback, or support:

**Mohammed Abdulrahman Alalyani**
- Email: [malredfan@gmail.com](mailto:malredfan@gmail.com)
- Instagram: [@malredfan](https://instagram.com/malredfan)
- X: [@malredfan](https://x.com/malredfan)
- LinkedIn: [malredfan](https://linkedin.com/in/malredfan)
