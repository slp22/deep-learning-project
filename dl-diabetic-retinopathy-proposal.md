#### Deep Learning | Project Proposal

# Lung X-Rays   

## Question
* What is the question behind your analysis or model and what practical impact will your work have?
    * How well can a neural network diagnose diabetic retinopathy?  
* Who is your client and how will that client benefits from exploring this question or building this model/system?
    * The client, the National Eye Institute, part of the National Institutes of Health, wants a model that can identify [diabetic retinopathy](https://www.nei.nih.gov/learn-about-eye-health/eye-conditions-and-diseases/diabetic-retinopathy) cases in [clinical trials](https://iovs.arvojournals.org/article.aspx?articleid=2565675). 

## Data Description
* What dataset(s) do you plan to use, and how will you obtain the data? 
    * Kaggle: [Diabetic Retinopathy](https://www.kaggle.com/datasets/sachinkumar413/diabetic-retinopathy-preprocessed-dataset)
    * n = 13,970
    * 5 classes (stages of [diabetic retinopathy](https://www.nei.nih.gov/sites/default/files/health-pdfs/diabeticretino.pdf)):
        * Normal eye
        * *Mild Nonproliferative Retinopathy*: microaneurysms,small areas of balloon-like swelling in the retina's tiny blood vessels. 
        * *Moderate Nonproliferative Retinopathy*: some blood vessels that nourish the retina are blocked.
        * *Severe Nonproliferative Retinopathy*: more blocked blood vessels, depriving several areas of the retina of blood supply; retina sends signals to the body to grow new blood vessels for nourishment.
        * *Proliferative Retinopathy*: advanced stage, new blood vessels are abnormal and fragile; grow along the retina and along the surface of the clear, vitreous gel that fills the inside of the eye. 
* What is an individual sample/unit of analysis in this project?
    * One retinal image (.jpg format)
* What characteristics/features do you expect to work with?
    * Image pixel, 3 rgb channels, height x width of image
* If modeling, what will you predict as your target?
    * Classify each image as one of five classes: normal, mild, moderate, proliferative, or severe. 
    
## Tools
* How do you intend to meet the tools requirement of the project?
    * Python, numpy, pandas, sklearn 
    * TensorFlow/Keras
* Are you planning in advance to need or use additional tools beyond those required?
    * None at this time.

## MVP Goal
* What would a minimum viable product (MVP) look like for this project?
    * simple neural network classification of 1 of 2 classes
    