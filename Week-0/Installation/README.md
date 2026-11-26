# Installation

## Goal

Set up an Ubuntu development environment (native Ubuntu), build NS-3 from source, run `hello-simulator`, and install the project Python packages. Use the official installation pages below because OS, hardware, and package commands can differ.

## Recommended order

1. **Ubuntu:** Follow Ubuntu's install guide. For NS-3, use Ubuntu's supported LTS release and keep the project environment inside the Linux filesystem.
2. **Build NS-3:** Follow the official NS-3 Installation Guide and Tutorial. Install the listed build prerequisites, obtain a source release, configure/build it, then run the `hello-simulator` example using the command shown by the tutorial for that release. Record the NS-3 release and exact command used; commands can vary across releases.
3. **Python 3.10+:** Install Python 3.10 or newer. On Ubuntu, use the distro's Python packages or a Python version manager; make a project virtual environment (`python3 -m venv .venv`) and activate it before installing Python libraries. Avoid installing project packages into the OS-managed Python environment.
4. **Install packages:** Use the official PyTorch selector to choose the correct CPU/CUDA command for your OS and hardware. In the activated virtual environment install Gymnasium, NetworkX, NumPy, Pandas, Matplotlib, and either `highspy` or SciPy. SciPy's `linprog(method="highs")` uses the HiGHS solver, so either option satisfies the LP tooling requirement.
5. **Verify:** Run `python --version`, import each library, print its version, and confirm the HiGHS route you chose imports. Keep the output in your submission.

## Official documentation and downloads

| Component | Official resource |
|---|---|
| Ubuntu Desktop download | [Ubuntu download page](https://ubuntu.com/download/desktop) |
| Install Ubuntu Desktop | [Ubuntu install tutorial](https://ubuntu.com/desktop/docs/en/latest/tutorial/install-ubuntu-desktop/) |
| NS-3 download/build/run | [NS-3 Installation Guide](https://www2.nsnam.org/docs/installation/) and [NS-3 documentation/tutorial index](https://www2.nsnam.org/documentation/) |
| Python | [Python downloads](https://www.python.org/downloads/) and [Python documentation](https://docs.python.org/3/) |
| PyTorch | [Official local install selector](https://pytorch.org/get-started/locally/) |
| Gymnasium | [Gymnasium documentation and install instructions](https://gymnasium.farama.org/) |
| NetworkX | [Install NetworkX](https://networkx.org/documentation/stable/install.html) |
| NumPy | [Install NumPy](https://numpy.org/install/) |
| Pandas | [Install Pandas](https://pandas.pydata.org/docs/getting_started/install.html) |
| Matplotlib | [Install Matplotlib](https://matplotlib.org/stable/install/) |
| HiGHS Python interface | [HiGHS `highspy` guide](https://ergo-code.github.io/HiGHS/stable/interfaces/python/) |
| SciPy LP interface (alternative) | [SciPy `linprog` with HiGHS](https://docs.scipy.org/doc/scipy/reference/optimize.linprog-highs.html) |

## Tasks

- Install Ubuntu.
- Install NS-3, build it, and run `hello-simulator`.
- Install Python 3.10 or newer and create a virtual environment.
- Install PyTorch, Gymnasium, NetworkX, NumPy, Pandas, Matplotlib, and `highspy` or SciPy.
- Record your OS/Python/NS-3 versions and successful command output.

Do not commit virtual environments, downloaded NS-3 source trees, or large generated build artifacts.
