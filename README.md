DataGotham.jl
=============

These IJulia notebooks provide the material used for the [Julia tutorial at DataGotham 2013](http://www.datagotham.com/tutorials/). To follow along, you'll need to install all of the software we use along the way:

_Step 1_: Grab a binary of the latest Julia from [http://julialang.org/downloads/#beta](http://julialang.org/downloads/#beta). If the binaries do not work, please install from source. The initial source installation takes a long time because of the dependencies that have to be installed, but subsequent builds takes less than a minute on average.

_Step 2_: For convenience, you can set up an alias to the newly installed Julia binary that you can use to invoke Julia from your normal shell prompt. On OS X, I use the following:

	alias julia="/Applications/Julia-*.app/Contents/Resources/julia/bin/julia"

I also setup an alias for IJulia to make it easier to launch:

	alias ijulia="ipython notebook --profile=julia"

_Step 3_: To get all the packages we'll use, start a Julia REPL and then run the following commands in the Julia REPL:

	Pkg.add("Homebrew")
	Pkg.add("IJulia")
	Pkg.add("Gadfly")
	Pkg.add("RDatasets")
	Pkg.add("GLM")
	Pkg.add("Optim")
