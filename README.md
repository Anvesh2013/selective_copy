# Selective Copy
[![Python Version](https://img.shields.io/pypi/pyversions/slcp.svg)](https://www.python.org/downloads/release/python-370/)
[![PyPi Version](https://img.shields.io/pypi/v/slcp.svg)](https://pypi.org/project/slcp/)
[![License](https://img.shields.io/github/license/pltnk/selective_copy.svg)](https://choosealicense.com/licenses/mit/)

Simple command line application that copies all files with given extension from a directory and its subfolders to another directory showing progress bar and remaining files counter.\
Allows to preserve a source folder structure and to create a log if necessary.\
Opens a filedialog if source and/or destination are not given in the command line.\
Creates folders in a destination path if they don't exist.

## Installing

<pre>
pip install slcp
</pre>

## Usage

<pre>
slcp ext [-s SRC] [-d DST] [-sc | -dc] [-p] [-l] [-h]

Positional arguments:
ext                     Extensions of the files to copy, enter without a dot, separated by commas.

Optional arguments:
-s SRC, --source SRC    Source folder path.
-d DST, --dest DST      Destination folder path.
-sc, --srccwd           Use current working directory as a source folder.
-dc, --dstcwd           Use current working directory as a destination folder.
-p, --preserve          Preserve source folder structure.
-i, --invert            Inverts the extension list. Copies everything except extensions you provided.
-l, --log               Create and save log to the destination folder.
-h, --help              Show this help message and exit.
</pre>

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details

## Acknowledgments

Inspired by the task from [Chapter 9 of Automate the Boring Stuff](https://automatetheboringstuff.com/chapter9/).
