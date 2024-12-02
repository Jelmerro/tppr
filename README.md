tppr
====

Tiny Portable Python Runner for hassle-free venv and dep handling

## About

This is a tiny command-line bash script to create and update venv versions.
It will check if an existing venv (virtual env) is present and use that to run the Python script.
If there is no venv yet, or the Python version is not up to date in the venv,
a new venv will be created in place of the old one.
After that the requirements file and the base directory are installed to the venv.
Finally, the Python script provided is ran with the venv activated.

## Usage

Download and store the `tppr` bash script anywhere in your PATH,
for example, you could run this command to put in in `~/.local/bin`:

```bash
curl -L https://raw.githubusercontent.com/Jelmerro/tppr/refs/heads/master/tppr -o ~/.local/bin/tppr
chmod +x ~/.local/bin/tppr
```

Once installed, simply run `tppr` with a Python script as an argument.
This will install Python and all the deps inside a venv and run the script.
For example `tppr ~/projects/example/file.py <args>`, with args all passed to the Python script.

## License

tppr was made by [Jelmer van Arnhem](https://github.com/Jelmerro) and is MIT licensed, see LICENSE for details.
