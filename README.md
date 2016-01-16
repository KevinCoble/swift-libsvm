# swift-libsvm
Port of LIBSVM code to Apple's swift language

All SVM code is from the public domain LIBSVM repository
See https://www.csie.ntu.edu.tw/~cjlin/libsvm/ for more information

LIBSVM features not supported:
    Sparse matrix input (but this allows the Accelerate library to be used),
    Pre-computed kernels,
    kernel caching,
    'shrinking',

Most other features are supported.  Features/options are set by setting attributes on the SVMModel class

The data is provided by a 'DataSet' class I created for a machine learning library.  The SVMTests.swift file shows examples of data set creation, training, and subsequent classification of data.  It also has (commented out) examples of storing/retrieving SVM models to disk files
