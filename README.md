# MedART

### Conception 
My friend is studying medicine and she has put a lot of effort into creating medical drawings during her education. I didn't want all of her hard work to go to waste, so it inspired me to start this project. I selected the most interesting drawings, scanned them, and created a strange dataset. Then, I applied my computer science skills and tried to use a neural network to transform your drawings.t. For me, it is a very complex process focused on creativity and extensive internal research.  The network SD 1.5 used in this project was fine-tuned. The image interpolation function describes data taken from EEG.

![frame_1161_SR](https://user-images.githubusercontent.com/39826275/220872948-9ae268f0-fc75-4fb3-ada8-b04884edfe45.png)
### Details
I submitted each photo 20 times to VAE from stable diffusion and after a special algorithm for finding neighbors, I arranged the photos by similarity 1-20 20-1, always finding the closest neighbor either in the acid version or in the normal one. The transition by drawings is implemented using the vector interpolation function in the latent space vae.

the dataset after passing through the processing pipeline looks like this

![output_gif_SD](https://user-images.githubusercontent.com/39826275/220875507-84bfcd01-fe9b-4d63-bf24-865cfbb9f9e5.gif)

And next stage i use img2img from fine tuned stable diffusion and procces every frame with a some specific prompt.

![output_gif](https://user-images.githubusercontent.com/39826275/220875889-3b8c6ba8-349f-4ad4-bcc1-a2726efe5acd.gif)

full result to large and you can download it from my link https://disk.yandex.com/i/To-UohJhqo5Q_Q

every img from this genetation available here https://disk.yandex.com/d/IYHuDjPCTK4FaQ
