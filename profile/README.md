# Hello Performance Team! :rocket:

This is Echoenergia's Performance team GitHub page. Here we have repositories for the main codes used by the team, most of them being in the format of python packages that can easily be installed using pip.

Feel free to contribute :smiley:! All code that at some point can be reused by someone is recommended to be in here for better version control. Just be sure to document your code as well as possible (look [here](https://realpython.com/documenting-python-code/) for good guidelines on how to document python code).

Please check out the [Documentation](https://github.com/performance-echo/documentation) section. A lot of useful information can be found there.

## Packages :package: 

Currently we are usyng Python :snake: version 3.12. Before installing the packages make sure that's the version you have installed. To do so, run the following command:

```bash
conda install python=3.12
```

You can install all echo pacakges at once using the command below. Add `--upgrade` to the second line if you also want to upgrade dependencies. 

```bash
uv pip install --force-reinstall --no-deps -r https://raw.githubusercontent.com/performance-echo/.github/main/echo_packages.txt
uv pip install -r https://raw.githubusercontent.com/performance-echo/.github/main/echo_packages.txt
```
> [!NOTE]
>
> - The command above uses uv for faster installs. If you don't have it installed, install it using `pip install uv`. After that you can always use `uv pip` for faster installs than regular `pip`.
> - If you are having trouble with the packages, specially after a Python version upgrade, run the second line of the command above adding the flag `--force-reinstall` at the end.

