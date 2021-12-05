# cipher
Scripts to ease ciphering and deciphering of files and folders

## Installation

Dependencies are:
- gpg
- pv
- tar

To install, clone repository and add `ci` and `de` to your PATH by copying or symlinking the files to, for example, /usr/local/bin.

## Usage

Create ciphered files/folders:

`ci -o folder/for/the/output/files -r recipient1 -r recipient2 file1 file2 folder1 folder2`

Deciphering files and folders:

`de -x -o folder/for/the/output/files file1.gpg file2.gpg folder1.tar.gz.gpg folder2.tar.gz.gpg`

`-x` is used to automatically extract .tar.gz.gpg files
