# QIR Generation
In this section, we will explore the generation of QIR from various development frameworks such as Q#, QuTip, and Qiskit. To demonstrate this process, we will use the example of teleporting the binary representation of "Hello World!" and emitting the QIR of the corresponding hybrid instruction. The teleportation protocol is heterogeneous, comprised both classical and quantum instructions. The interdependent conditionals following the measurement of the message and the auxiliary qubits in teleportation determine the next quantum gate operations on the target qubit.
For python-based frameworks we can utilize [PyQIR](https://github.com/qir-alliance/pyqir) APIs to generate QIR. In the case of Q#, the QIR generation is built into the compiler. There are two options for emitting QIR from Q#: the use of the magic command within a [Jupyter notebook](qir-book/tutorials/qir-emission/qsharp/in_jupyter/qsharp-magic.ipynb), or [setting](https://github.com/microsoft/qsharp-compiler/blob/main/examples/QIR/Emission/Emission.csproj) the QIR XML tag in the C# project file.