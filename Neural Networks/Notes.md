http://www.wildml.com/2015/09/

Neural Network from Scratch
https://github.com/dennybritz/nn-from-scratch/blob/master/nn-from-scratch.ipynb

Neural Network using Theano GPU
    Install: (http://rianadam.web.ugm.ac.id/2016/04/07/install-theano-on-windows-10/)
        Visual Studio 2013
        Cuda 7.5
        Anaconda2 for Python 2.7 x64
        Microsoft Visual C++ Compiler for Python 2.7 (https://www.microsoft.com/en-us/download/confirmation.aspx?id=44266)
        conda install mingw libpython
        pip install theano
        
        Download cudnn-7.5-windows10-x64-v5.1-rc
        Extract and copy all the files to C:\Program Files\NVIDIA GPU Computing Toolkit\CUDA\v7.5
        
        Create .theanorc.txt file
            [global]
            floatX = float32
            device = gpu

            [lib]
            cnmem=1000

            [nvcc]
            flags=-LC:\Users\Jess\Anaconda2\libs
            compiler_bindir=C:\Program Files (x86)\Microsoft Visual Studio 12.0\VC\bin\cl.exe

            [cuda]
            root=C:\Program Files\NVIDIA GPU Computing Toolkit\CUDA\v7.5

Do not install pydot. Some conflicts with theano. Generate "gof" error