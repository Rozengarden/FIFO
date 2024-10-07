# Fork Around, Find Out

A collection of on-chain adventure, exploring various features of Defi protocol

## Requirement and installation

Make sure to have `git` installed

### Foundry

To easily fork (make a local "copy" we can modify without impacting the real world) the blockchain we are going to need `foundry`.
There are many way to do it, all described on [getfoundry.sh](https://book.getfoundry.sh/getting-started/installation)

If openig a link is too much for u here is an easy way:

```
curl -L https://foundry.paradigm.xyz | bash # rember that blindly downloading stuff from the net is not a good practice
foundryup
```

### Pyenv (optional)

This tools allow to manage multiples version of python on ur machine and seamlessly use them based on ur working directory.
U can skip it if u want to manage it urself.
Here is the complete [instruction](https://github.com/pyenv/pyenv?tab=readme-ov-file#installation)

And here if u lazy:
```
curl https://pyenv.run | bash
```

Once installed we are going to use it to setup a python version for ape

```
pyenv install 3.12
pyenv global 3.12 # optional, it set up python system wide
pyenv virtualenv 3.12 ape
```

### Ape

U will need to have `python` and `pip` installed, `pyenv` can do that for u but if u skipped it it's on u ur on ur own :p

Go into a folder where u store all ur project and clone this repo and setup ape

```
git clone https://github.com/Rozengarden/FIFO.git
cd FIFO/
pyenv local ape # only if u installed python via pyenv
pip install eth-ape'[recommended-plugins]'
ape plugin install . # this will instal moar plugin if needed
```

U are now ready for an onchain adventure.


