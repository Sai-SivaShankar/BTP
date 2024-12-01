**Reconstructing CT Images Efficiently with Advanced Techniques**

In X-ray computed tomography (CT), images are reconstructed from incomplete and noisy data called **sinograms**. Traditional methods like **Filtered Back Projection (FBP)** have been widely used but struggle with sparse or noisy data, leading to suboptimal image quality. 

Recent advancements in deep learning, particularly **deep unrolling networks**, have significantly improved image reconstruction, making them the current state-of-the-art. These networks blend traditional iterative algorithms with learnable neural networks, offering both improved performance and interpretability. However, they face challenges, especially in 3D imaging, due to:
- **High computational costs**: Repeated use of full forward and adjoint operators at each network layer.
- **Scalability issues**: These methods become impractical for high-dimensional tasks.

To address these challenges, **stochastic primal-dual (SPD)** and **sketched learned stochastic primal-dual (SL-SPD)** networks have been proposed (Tang, Mukherjee, and Schönlieb, 2022). These methods offer a balance between computational efficiency and reconstruction quality by:
1. Reducing the reliance on full operators at every step.
2. Leveraging stochastic approximations and sketching techniques.

Experiments show that SPD and SL-SPD achieve reconstruction quality comparable to the **Learned Primal-Dual (LPD)** network (Adler & Öktem, 2018) but at significantly lower computational costs. This makes them a promising alternative, particularly for large-scale 3D CT reconstruction tasks.

![image](https://github.com/user-attachments/assets/c1170d64-b62a-4736-ab65-a7d483ffb1fa)
![image](https://github.com/user-attachments/assets/f92c5dd0-5297-489c-ad18-664cac392ea7)
![image](https://github.com/user-attachments/assets/15f58bf3-823a-4427-88d1-85ab578845e7)
