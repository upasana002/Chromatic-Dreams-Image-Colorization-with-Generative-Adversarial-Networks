# Chromatic-Dreams-Image-Colorization-with-Generative-Adversarial-Networks

# PROBLEM STATEMENT -
Traditional methods often struggle to produce realistic and vibrant colors, especially in complex scenes or with subtle details. In this context, leveraging Generative Adversarial Networks (GANs) presents a promising avenue for enhancing the quality and fidelity of colorization results. However, existing GAN-based approaches encounter issues such as color consistency, artifacting, and computational inefficiency. Thus, there is a pressing need to develop novel techniques that effectively address these challenges and push the boundaries of image colorization with GANs, ultimately enabling the creation of lifelike and visually appealing colorized images across various domains and applications.

DATASET : https://drive.google.com/drive/folders/12hEx4LSPaTEw_96I8nlncJSPY5u1FXn4?usp=sharing

MOTIVATION - 
Recolorizing and restoring old photos is a painstaking process when done manually through some photo editing software.
One solution to this problem is using GANs . 
Colorizing black and white images with deep learning has become an impressive showcase for the real world application of neural networks in our lives.


PYTHONFILE- : https://colab.research.google.com/drive/1c47yo6VuF7CabDvmZBGfYrOY5tE1_XNV?usp=sharing

WHAT ARE GAN’S -
Generative Adversarial Networks ( GANs) are a way to make generative models by having two neural networks compete with each other . GANs are the state-of-the-art machine learning models which can generate new data instances from existing ones. They use a very interesting technique, inspired from Game Theory, to generate realistic samples

Source : https://www.techtarget.com/searchenterpriseai/definition/generative-adversarial-network-GAN

METHODOLOGY - 

1. Dataset Description:
The dataset comprises 3000 RGB images sourced from various domains, including landscapes such as mountains, forests, urban scenes, and more. These images serve as the foundation for the training process.

2. Preprocessing:
RGB images are converted into grayscale to serve as the ground truth labels for the model. This conversion simplifies the task, focusing solely on learning the colorization process without the complexity of full-color images.

3. Training Strategy:
The training strategy alternates between updating the generator once and the discriminator twice for each training step.

4. Discriminator Objective:
The discriminator aims to accurately classify generated images as fake or real and assign high probabilities (closer to 1.0) for images originating from the dataset. This objective ensures effective discrimination between real and fake images, providing meaningful feedback to the generator.

5. Generator Objective:
The generator minimizes its loss by producing images that deceive the discriminator. Generating images indistinguishable from real ones "fools" the discriminator into assigning high probabilities to its outputs, even though they are artificially generated.

6. Training the Discriminator:
The discriminator is iteratively trained to discern real images from fake ones, outputting probabilities closer to 1.0 for real images and closer to 0.0 for images generated by the generator. This adversarial training process enhances the discriminator's ability to distinguish between real and fake images.

7. Adversarial Training:
Through adversarial interplay between the generator and the discriminator, the goal is to elevate the quality of generated images progressively. As the generator improves, it challenges the discriminator to become more discerning, leading to continuous improvement in both components.


8. Optimization Goal:
The optimization goal is to train a generator capable of producing high-quality colorized images resembling real-world scenes. By refining the generator's ability to deceive the discriminator, the aim is to achieve visually compelling colorization results across diverse domains.


CONCLUSION-
In summary, the approach employing Generative Adversarial Networks (GANs) for image colorization demonstrates considerable promise in generating high-fidelity colorized images. The dataset comprising 3000 RGB images, preprocessed into grayscale for labeling, serves as a robust training corpus. The iterative training process, with alternating updates between the generator and discriminator, fosters the gradual enhancement of the generator's proficiency in producing realistic colorizations while continually challenging the discriminator's discernment capabilities. By employing the L2/MSE loss function and the Adam optimizer with a learning rate of 0.0005, the training process ensures stable and efficient convergence. Overall, this methodology presents a significant stride in advancing image colorization techniques, paving the way for the creation of visually captivating and authentic colorized images across diverse domains.
