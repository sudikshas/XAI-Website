---
layout: page
title: Web Application
permalink: /webapp/
---
<body>
    <p><b>Static Demo: <a href="https://nicole9925.github.io/facial-analysis-frontend/">LINK</a></b></p>
    <p><b>Undeployed Web Application with full functionality: <a href = "https://github.com/nicole9925/facial-analysis-webapp">GITHUB REPOSITORY</a></b></p>
    <br>
    <br>
    <iframe width="840" height="630"
        src="https://www.youtube.com/embed/Ri2yRwkdSS0">
    </iframe>
    <p>
        After finishing all of the parts to our project, we assembled our results into an interactive web application to share to the public.
        <br>
        <img src="https://github.com/michael4706/XAI_Website/blob/master/getImage.png?raw=true" alt="Home Page" width="420" height="315">
        <br>
        The web application welcomes the user a homepage that consists of visualizations of our dataset's distribution, background information, and dataset information. Upon submitting an image, the user will be brought to the prediction page that lists our predictions for the face's gender, age, and race, along with corresponding graph visualizations of the results.
        <img src="https://github.com/michael4706/XAI_Website/blob/master/Prediction.png?raw=true" alt="Predictions" width="420" height="315">
        <br>
        The next page show three types of visualizations that correspond to the predictions from the previous page. The user may click on the buttons to change the visualizations shown.
        <br>
        <img src="https://github.com/michael4706/XAI_Website/blob/master/Grad.png?raw=true" alt="Grad-CAM" width="210" height="150">
        <img src="https://github.com/michael4706/XAI_Website/blob/master/BP.png?raw=true" alt="Back-Propagation" width="210" height="150">
        <img src="https://github.com/michael4706/XAI_Website/blob/master/IG.png?raw=true" alt="Integrated Gradients" width="210" height="150">
        <br>
        We then discuss how racial bias in training machine learning models can visually affect output images with examples. Captions are displayed upon hover. Additionally, we display visualizations of the accuracy in relation to race. Lastly, we end with a conclusion.
        <br>
        <img src="https://github.com/michael4706/XAI_Website/blob/master/Bias.png?raw=true" alt="Bias" width="300" height="210">
        <img src="https://github.com/michael4706/XAI_Website/blob/master/Conclusion.png?raw=true" alt="Conclusion" width="300" height="210">
        <br>
        Due to limitations of using free tier on hosting platforms, we were not able to deploy the backend of our application. To view a static conceptual site (with a default image), you can visit <a href="https://nicole9925.github.io/facial-analysis-frontend/">here</a>. Please visit this <a href = "https://github.com/nicole9925/facial-analysis-webapp">our github repository</a> to locally run our web application with full functionality. The instructions to run are listed in the readme. 
    <br>
        Nonetheless, our application is fully deployable upon upgrading your heroku account. If you would like to deploy it, please visit <a href = "https://github.com/nicole9925/facial-analysis-frontend/tree/master">frontend</a> and <a href = "https://github.com/nicole9925/facial-analysis-backend">backend</a> repositories on GitHub for more information.
    </p>
</body>
