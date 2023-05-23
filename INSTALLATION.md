# Installation through opam (Mac & Linux)

OPAM is the package manager for the Ocaml programing language. 

On linux, simply go for `sudo apt-get install opam` to install it, and on Mac go for `brew install opam` or `port install opam`.

After installing opam, simply run `opam install cryptoverif` and you should obtain a fully executable cryptoverif.

See https://opam.ocaml.org/doc/Install.html for details on the opam instalation if needed.

# Getting the executable for Windows

Simply download the zip file at https://bblanche.gitlabpages.inria.fr/CryptoVerif/cryptoverifbin2.06.zip, which contains a .exe.

# Cross platform using docker

After installing docker with either full GUI desktop interface (https://docs.docker.com/desktop/) or only the engine (https://docs.docker.com/engine/install/), proceed with pulling the image at https://hub.docker.com/r/cjacomme/cryptoverif.

Under MAC or Linux, one can use a shell to execute `docker pull cjacomme/cryptoverif`, a bash whitin the docker is then obtained with ` docker run -it -v $(pwd):/home/examples cjacomme/cryptoverif bash
` (this command should be executed from a directory containing the files you want to run cryptoverif on, as the current folder will be mounted inside the docker).

Under windows, you will have to clic through the desktop application. 

# Manual installation (Linux, maybe Mac)

If you do not want to use the builtin docker or opam, here are some instructions for manual installation. They are based
on Ubuntu, but you might be able to adapt them for your OS.

* Download the cryptoverif sources at https://cryptoverif.inria.fr/cryptoverif2.06.tar.gz
* Create the target directory `mkdir cryptoverif`
* Unpack the sources `tar -xzf cryptoverif2.06.tar.gz -C cryptoverif --strip-components=1`
* Install the dependencies:
  * `sudo apt-get install m4 ocaml opam zlib1g-dev`
  * `opam install ocaml ocamlfind cryptokit conf-m4`
* Then, execute the `./build` script in unpacked the CryptoVerif directory.
* Add the current folder to your path, typically with `export PATH=~/cryptoverif:$PATH`


# License

Of course, you MUST take notice of the license file at https://bblanche.gitlabpages.inria.fr/CryptoVerif/cryptoverif.html before using it.
