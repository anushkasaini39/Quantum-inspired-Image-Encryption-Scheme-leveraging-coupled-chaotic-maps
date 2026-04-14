# Quantum-Inspired Image Encryption Using Coupled Chaotic Maps

As medical devices become more connected via the Internet of Medical Things (IoMT), securing 
medical image data from unauthorized access and tampering has become a critical concern. Many 
existing technologies are unable to maintain a balance between computational efficiency and 
strong encryption, especially when high-quality reconstruction of diagnostic images is necessary. 
This paper proposes SecureMed, a fast and computationally efficient encryption technique for 
secure medical image transmission. SecureMed uses an attention-augmented overcomplete 
autoencoder (AAOA) to extract high-fidelity dual-channel latent features, which are then secured 
through a five-stage encryption framework: quantum-inspired amplitude encoding to project data 
into a Hilbert space, coupled chaotic modulation, Hadamard diffusion, Hilbert curve permutation 
to induce spatial rearrangement paired with orthogonal random matrix diffusion, and a terminal 
cumulative bit-level XOR diffusion. As a result, the encrypted image becomes highly randomized 
and distorted, preventing unauthorized analysis. It follows symmetric decryption operations 
for accurate recovery of the encrypted image data. Experimental results demonstrate that 
SecureMed achieves high reconstruction fidelity, reflected by an average 63.892 dB PSNR and 
0.9999 SSIM, and a significant reduction in adjacent pixel correlation in the ciphertext to about 
0.0029. It exhibits a massive key space of  2637 with a key sensitivity of 10-16, due to which the 
brute-force attacks are computationally infeasible. Security metrics confirm its strong resistance 
against statistical and differential attacks, reflected by an ideal 99.61% NPCR, 33.46% UACI, and 
7.99 Entropy, demonstrating its encryption efficacy and performance comparable with state-of
the-art techniques. The scheme offers a scalable method to secure healthcare data in resource
constrained and dynamic IoMT settings.
