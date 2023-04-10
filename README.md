# A CLI for Interacting with ChatGPT

Requires Python 3.10

## Instructions

Get your API key from [https://platform.openai.com/account/api-keys](https://platform.openai.com/account/api-keys).

Make a copy of .env.example as .env and copy your API key into it.

Run `pip install -r requirements.txt`. This might take a while since this will install EasyOCR. You can edit the query script to remove this if it's not used.

Install pandoc if you need to extract text from docx files as well. Refer to [https://pypi.org/project/pypandoc/])(https://pypi.org/project/pypandoc/)

Move your data, e.g. pdf files or txt files to the data subfolder. You can try it with alice30.pdf (provided).

If you wish to add webpages to your list of sources, edit `inventory.json` and add your urls there.

Run `./query "<question>"`, e.g. `./query "What is this story about?"`.

If you encounter issues running the script in this way, you might need to edit the hash-bang line at the top of the query file to get it to use the right executable. Currently it defaults to `python3.10`.

