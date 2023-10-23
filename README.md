# Self-Learning Activation Functions to Increase Accuracy of Privacy-Preserving Convolutional Neural Networks with Homomorphic Encryption

Homomorphic Encryption (HE) emerges as a mechanism for expanding the scope of public cloud services for sensitive data processing. HE describes a special form of encryption with the capability of performing certain operations over ciphertexts without using the secret key. The information can be public without representing a risk of a data breach. The output of the calculated functions remains encrypted and maintains the input format. Its correctness relies on the homomorphism concept, where two groups in different spaces can be mapped. In this case, a homomorphic function applied to ciphertexts provides the same result (after decryption) as applying the function to the original unencrypted data.

However, high-demand solutions such as neural networks require efficient operations beyond HE additions and multiplications. The state-of-the-art solutions have been focused on implementing cryptographically compatible activation functions. In this paper (link to be added upon publication), we propose a method to increase the accuracy and performance of privacy-preserving Convolutional Neural Networks with Homomorphic Encryption (CNN-HE) by Self-Learning Activation Functions (SLAF). SLAFs are polynomials with trainable coefficients updated during training, together with synaptic weights for each polynomial independently to learn task-specific and CNN-specific features. This project includes the source code used in this study. For additional information, refer to (link to be added upon publication). 

The [Cheon-Kim-Kim-Song (CKKS)](https://doi.org/10.1007/978-3-319-70694-8_15) HE scheme and homomorphic operations were implemented using the open-source Simple Encrypted Arithmetic Library (SEAL) through the Python [TenSEAL](https://github.com/OpenMined/TenSEAL/) library. The ciphertext size, scheme performance, multiplicative depth, and security level directly depend on the security parameter settings. We adopt security settings specified in the [HE standard](https://HomomorphicEncryption.org/standard).

The project includes four Jupyter notebooks:
- CNN1_HE_SLAF.ipynd: Training and testing CNN1-HE-SLAF model.
- CNN2_HE_SLAF.ipynd: Training and testing CNN2-HE-SLAF model.
- Performance_accuracy_comparison_approaches.ipynb: Performance of the state-of-the-art fixed-precision numbers homomorphic comparison approaches.
- Interval_based_approximation_analysis.ipynb: Interval-based error analysis of fixed-precision numbers homomorphic comparison approaches.

For assistance with this source code, please contact us at lpulido@cicese.edu.mx
