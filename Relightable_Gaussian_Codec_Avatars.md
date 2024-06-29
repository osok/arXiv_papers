# SUMMARY

The authors discuss the challenges of creating real-time, photorealistic avatars due to the complex materials and geometry of human heads. They propose a learning framework using 3D Gaussians, a relightable appearance model, and an explicit eye model to achieve accurate scattering and reflections.

# IDEAS:

- Human heads have complex materials with unique scattering and reflectance properties.
- Real-time relighting of human heads is challenging due to diverse material properties.
- Skin reflects light in complex ways due to microgeometry and subsurface scattering.
- Hair scatters light out of plane and reflects it multiple times.
- Eyes have multiple layers and highly reflective membranes, adding complexity.
- No single material representation can accurately depict all head elements in real time.
- Tracking and modeling head geometry in motion is a daunting task.
- Real-time rendering constraints limit algorithmic design for photorealism.
- The authors propose a learning framework for real-time renderable head avatars.
- The framework uses 3D Gaussians for geometric representation.
- A relightable appearance model based on learned Radiance transfer is used.
- An explicit eye model allows separate control of gaze and facial movements.
- The combination of 3D Gaussians and the relighting appearance model outperforms other methods.
- Facial Avatar modeling has been researched for over 50 years.
- Image-based 3D reconstruction allows for more precise facial feature acquisition.
- Existing shape representations struggle with modeling thin structures like hair strands.
- Relighting methods often lack photorealism and do not support novel animations.
- The proposed method integrates target illumination into the neural decoder.
- Data was collected using high-resolution images from multiple angles with 110 cameras and 460 LED lights.
- Participants performed various facial expressions and eye movements for data collection.
- The geometric representation uses a mixture of 3D and isotropic Gaussians.
- The final color at each pixel is computed using point-based cumulative volumetric rendering.
- A conditional variational autoencoder (CVAE) learns the distribution of facial expressions.
- The appearance model captures various light transport effects like subsurface scattering and specular reflections.
- The diffuse term is based on spherical harmonics, incorporating global light transport effects.
- The specular term uses a spherical Gaussian to achieve sharp mirror-like reflections.
- An explicit eye model parameterizes eyeballs as a blend of two spheres representing the eyeball and cornea.
- The model is trained using multi-view video data with known point light patterns.
- The model is evaluated on diverse subjects using metrics like PSNR, SSIM, and LPIPS.
- The proposed method supports real-time relighting and high-fidelity breakdown of intrinsic properties.

# INSIGHTS:

- Real-time relighting of human heads requires detailed modeling of complex materials.
- Accurate tracking of head geometry in motion is essential for photorealism.
- A learning framework using 3D Gaussians can achieve real-time renderable head avatars.
- Relightable appearance models must support global light transport and all frequency reflections.
- Explicit eye models enable separate control of gaze and facial movements for photorealism.
- Integrating target illumination into neural decoders improves quality and simplifies learning pipelines.
- High-resolution multi-view data collection is crucial for diverse lighting conditions and stable facial tracking.
- Conditional variational autoencoders effectively learn the distribution of facial expressions for animation.
- Spherical harmonics and spherical Gaussians are key to capturing diffuse and specular light transport effects.
- Real-time relighting requires efficient rendering techniques like point-based cumulative volumetric rendering.

# QUOTES:

- "Human heads are made up of complex and diverse materials each with unique scattering and reflectance properties."
- "Skin reflects light in complex ways due to its microgeometry and significant subsurface scattering."
- "Hair with its translucent fiber structure scatters light out of plane and reflects it multiple times."
- "The eyes with their multiple layers and highly reflective membranes add another layer of complexity."
- "Accurately tracking and modeling the underlying geometry in motion is a daunting task."
- "The need for real-time rendering puts a severe constraint on the design of the algorithm."
- "Our aim is to create a learning framework that can construct real-time renderable head avatars."
- "We use exhaustive measurements from a light stage and physically based rendering methods."
- "Our geometric representation is based on 3D Gaussians that can be rendered in real time."
- "We use 2D convolutional neural networks to decode 3D Gaussians on a shared UV space."
- "For appearance, we've developed a relightable appearance model based on learnable Radiance transfer."
- "Our relightable Gaussian Avatar also incorporates an explicit eye model that enables explicit control of the eyeballs."
- "Facial Avatar modeling has been a topic of research for many years with advancements in image-based 3D reconstruction."
- "Existing shape representations struggle with modeling extremely thin structures like hair strands."
- "We propose to integrate a target illumination at the output of our neural decoder."
- "We collected our data using a setup similar to previous studies with high-resolution images from multiple angles."
- "Our geometric representation is based on a mixture of 3D and isotropic Gaussians."
- "We used a conditional variational autoencoder (CVAE) to learn the distribution of facial expressions from the data."
- "Our diffuse term is based on spherical harmonics and includes global light transport effects."
- "To achieve sharp mirror-like reflections for the view-dependent specular term, we use a spherical Gaussian."

# HABITS:

- Collect high-resolution multi-view images for diverse lighting conditions and stable facial tracking.
- Use conditional variational autoencoders to learn the distribution of facial expressions for animation.
- Integrate target illumination into neural decoders to improve quality and simplify learning pipelines.
- Employ spherical harmonics for diffuse light transport effects in appearance models.
- Utilize spherical Gaussians for sharp mirror-like reflections in specular light transport effects.

# FACTS:

- Human heads have complex materials with unique scattering and reflectance properties.
- Real-time relighting of human heads is challenging due to diverse material properties.
- Skin reflects light in complex ways due to microgeometry and subsurface scattering.
- Hair scatters light out of plane and reflects it multiple times.
- Eyes have multiple layers and highly reflective membranes, adding complexity.

# REFERENCES:

None mentioned.

# ONE-SENTENCE TAKEAWAY

Real-time photorealistic avatars require detailed modeling of complex materials, accurate geometry tracking, and efficient rendering techniques.

# RECOMMENDATIONS:

- Use 3D Gaussians for geometric representation in real-time renderable head avatars.
- Develop relightable appearance models supporting global light transport and all frequency reflections.
- Incorporate explicit eye models for separate control of gaze and facial movements in avatars.
- Collect high-resolution multi-view images for diverse lighting conditions and stable facial tracking.
- Employ conditional variational autoencoders to learn the distribution of facial expressions for animation.