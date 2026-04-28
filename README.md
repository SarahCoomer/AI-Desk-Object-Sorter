# AI Desk Object Sorter

## Project Description
In this project I will use https://teachablemachine.withgoogle.com/train/image to identify 3 different desk objects on my desk. 
## Classes Identified
List the objects your model was trained to identify:
* Class 1 Computer Mouse
* Class 2 Sticky Notes
* Class 3 Controller

### Discussion & Reflection

1.  **Model Performance & Iteration:**
    * How accurate was your first trained model?
        * My model performed well on the classes I trained it for. The computer mouse class output was 81%; sticky notes indicated a 0%; and the controller class output was 19%.
    * What steps did you take to iterate and improve its performance?
        * In order to iterate and improve, I added more images per class, with different angles, different distances, and different lighting with the environment around my desk.
    * How did these changes affect the model's accuracy and confidence scores?
        * This provided variations to train the model improved its accuracy and ability to identify the desk objects. In addition the model seemed to be able increase confidence scores on images where it struggled to discern between two classes. 

2.  **Challenges & Observations:**
    * Which objects were the easiest for your model to learn and distinguish? Why do you think that was?
        * The Xbox controller seemed the easiest for the model to learn in distinguish from. I think this is due to the form factor of the controller, its size was not similar to the mouse or sticky notes, and the silhouette is comparable to most gaming controllers.
    * Which objects were the most challenging? What made them difficult
         * The most difficult for the model was the computer mouse and sticky note pads. I believe this is due to similar size and color of the items. I realized after I trained the model, that all my objects were different shades of blue, and this contributed as well.
    * What happened when you showed the model an object it wasn't trained on? How did the confidence scores behave, and why is this significant?
         * When I showed the model a pen, it distributed confidence across all three classes. This is significant because it exemplifies that model does not understand the concept of "none of the above" as a correct answer. The model picks the closest class it can the original 3 classes because it still has to pick a provided class.  

3.  **Bias in AI:**
    * If you only trained your computer mouse class with images of your specific computer mouse (and didn't vary color, shape, etc.), how well do you think it would recognize other students' significantly different mugs? How does this illustrate the concept of bias being introduced through training data?
         * It would not recognize other computer mice. As it would fall prey to only recognizing the features specific to my particular computer mouse. This illustrates the concept of bias being introduced through training data as it teaches the model to recognize the features of a specific computer mouse and not the concept of the computer mouse.
    * Imagine all your training images were taken in very bright, direct lighting. What might happen if you tried to use the model in a dimly lit room or with strong shadows? How does this relate to the robustness and potential biases of AI models?
         * If I were to upload my image samples in a dimly lit room with strong shadows it would teach the model to associate the highlights and shadows as features of the object. This relates to robustness as it can cause the model to completely misclassify and drop confidence as it would shift the features and create a bias within the model. 

4.  **Model Limitations & Usefulness:**
    * What are some key limitations of the model you created?
         * It cannot choose any answer but the three classes, making a fourth object break the ability for it to classify.
         *  This type of model is sensitive to lighting, angles, and distance from the webcam, as it is unable to recognize 3-D objects
         * By taking pictures the model is only able to classify frames instead context over time.
    * Why is it useful to be able to download your trained model files (like `model.json`, `weights.bin`) and share them (e.g., via GitHub)? What does this enable?
         * Downloading and sharing these files enables someone else to be able to start where I stopped, and not have to re-train from scratch. Sharing to a github gives easy access and the ability to collaborate and reproduce my results. 

5.  **Real-World Applications & Ethics:**
    * Brainstorm 2-3 real-world applications where a similar image classification model could be useful.
         * Camera assisted vending machines
         * Translating ASL for the hearing impaired
         * Production sorting merchandise by size
    * Briefly discuss one ethical consideration that developers should keep in mind when building and deploying image recognition AI in the real world (e.g., related to fairness, privacy, misuse).
         * One ethical consideration that developers should keep in mind when building and deploying image recognition AI in the real world is representation. Developers must actively audit and rule out bias that pertains to what the object is and what the object represents before, during, and after deployment.

<img width="1261" height="999" alt="image" src="https://github.com/user-attachments/assets/e5ba4803-b5ef-40a0-8819-d84152d7664c" />
