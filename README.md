# Quantum-Inspired Image Encryption Using Coupled Chaotic Maps

Here we developed a lightweight encryption framework built for medical images. The goal is to secure the healthcare image data without damaging it.

It first converts Healthcare scans (like x-rays, CT scans,and MRIs etc.) into a continuous latent feature maps using an overcomplete attention-based autoencoder (no downsampling, so details stay intact). Then a multi-step pipeline— quantum encoding, chaotic mixing, Hadamard based diffusion, Hilbert scrambling, and random projections diffusion, cumulative xor diffusion—breaks any visible structure. 
End resultis encrypted images look completely random, but the original can be reconstructed exactly.

Our experimental metrics are soo cool, we got 
..look firstly, all encrypted images metrics should have low values ,approx 0, denotes degraded quality , except DEM,Entropy,NPCR,UACI(as they tells in laymen language- level of disorderness- so it should he higher..)
and vice versa for decrypted, nar to 1, and psnr should be above 45..

our framework achieved--

| Category             | Type of Metric        | Encrypted Image | Decrypted Image |
|---------------------|----------------------|-----------------|-----------------|
| Visual Quality      | PSNR                 | 7.7469 dB       | 63.8921 dB      |
|                     | SSIM                 | 0.0079          | 0.9999          |
|                     | CC                   | 0.0029          | 0.9788          |
|                     | VIF                  | 0.0052          | 0.9999          |
|                     | DEM                  | 0.8936          | 0.0253          |
----------------------------------------------------------------------------------
| Security Analysis   | Key Space            | 2^637           | -               |
|                     | Key Sensitivity      | 10^-16          | -               |
----------------------------------------------------------------------------------
| Differential Attack | NPCR                 | 99.6088%        | -               |
|                     | UACI                 | 33.4875%        | -               |
----------------------------------------------------------------------------------
| Statistical Analysis| Entropy              | 7.9972          | ~6  |
|                     | MSE                  | 11316.65        | ~0              |
