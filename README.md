# Toy models of predictive coding for dynamic spiking neural networks

## Supplementary code for the paper submitted to Neural Computation journal

 Authors: S. Sukhov, B. Batuev
 <br>
 Kotelnikov Institute of Radio Engineering and Electronics of RAS
 <br>
 2024

 ### General info
Simple architectures of dynamic spiking networks are presented that incorporate the elements of predictive coding for hierarchical control of dynamic systems. Integrators and coupled oscillators with predictive coding are constructed using populations of spiking leaky integrate-and-fire neurons. The dynamic neuronal models are implemented in the Nengo package.

 ### The files in the repository

`Predictive_integrator.ipynb`
 The error signal modifies the dynamics of the integrator of the upper hierarchical level and becomes zero when proper represented value is achieved. 

`PC_Nengo_PhaseSynch.ipynb`
The code demonstrates the synchronization of the master and the receiver oscillators using predictive coding and two types of errors.

`Predictive_coding_learning.ipynb`
Learning in Predictive Coding Network with Oscillators. The essence of the model is that two oscillators interact with each other through a learning mechanism (PES rule) to minimize the error between them.

## Usage
### Environment Setup

Prepare the environment with Python 3.10.13 and the required dependencies by running:

```bash
pip install 'nengo==3.2.0' 
pip install 'nengo-gui==0.5.0'
```

## References

- [Nengo Documentation](https://www.nengo.ai/nengo/)
- [Nengo Examples: Integrator](https://www.nengo.ai/nengo/examples/dynamics/integrator.html)
- [Nengo Examples: A simple harmonic oscillator](https://www.nengo.ai/nengo/examples/dynamics/oscillator.html)

## License

This code is provided under the [MIT License](LICENSE). Feel free to use, modify, and distribute it as needed. If you find it helpful, consider sharing your improvements with the community!