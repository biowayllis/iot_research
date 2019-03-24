# CAL- RAE / New Sun Road Battery Research

## Recommended setup
Make sure you have Python 3 installed; this guide for windows assumes that `py` will reference your Python3 distribution.
1. Create a virtual environment using `venv` (see [documentation](https://docs.python.org/3/tutorial/venv.html)). `py -m venv env`
2. Activate it: `env\Scripts\activate`. You'll have to do this every time
3. If querying Stellar:
    1. Install [stellar-client](https://github.com/cal-rae/stellar-client): `py -m pip install git+git://github.com/cal-rae/stellar-client.git`
    2. Create a file called `auth_config.py` and add a line with your Stellar stellar_token: `stellar_token='[your token]'`
4. Create a kernel for using in Jupyter notebooks (see this [guide](https://anbasile.github.io/programming/2017/06/25/jupyter-venv/)).
    1. Make sure your virtual environment is activated
    2. Install ipykernel: `py -m pip install ipykernel`
    3. Add a kernel for this project: `ipython kernel install --user --name=calrae-battery-research`
5. Install other tools you might need, e.g. matplotlib: `py -m pip install matplotlib`

You should be good to go. Fire up Jupyter Notebooks and navigate to this folder. Open the example notebook and select the `cal-rae-battery-research` kernel and run it.
