---
layout: page
title: Model
permalink: /model/
---

<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link href="https://michael4706.github.io/XAI_Website/style/style.css" rel="stylesheet" /> <!--/style/style.css-->
</head>

<body>
    <section class = "model">
            <h4><b>Convolutional Neural Network</b></h4>
            <p> 
                We used CNN as our model. We applied transfer learning with resnet50 by taking the first 14 layers and fixing
                their weights. Then, we concatenated them with our self-defined layers. We preprocessed the training images by 
                resizing it to 224 x 224 x 3 and applied the resnet_v2 input preprocessing function and adding random
                augmentation to our training data.
            </p>
            <h4><b>Model Parameters</b></h4>
            <p>
                The parameters for training are listed as follows: <b>batch size = 128, learning rate = 0.008,
                optimizer = Nadam, loss = categorical cross entropy</b>. The learning rate will iteratively decrease if
                the validation loss does not decrease for 10 consecutive epochs. The early stopping would be triggered if the
                validation loss does not decrease for 30 consecutive epochs.
            </p>
    </section>
    <section class = "Training Progress">
        <h4><b>Training Progress and Result</b></h4>
        <p>
            The plots below show the training progress of three models: race, age, and gender. From the plots, we can observe that
            the validation accuracy of gender is the highest, followed by race and gender. Considering the number of categories inside
            each class, the results are expected.
        </p>
        <h4><b>Race Model</b>(7 classes with 66% accuracy)</h4>
        <div class="race_row">
            <div class="race_progress">
                <img src="https://michael4706.github.io/XAI_Website/img/race/acc_curve.png" style="width:100%"> <!--/img/race/acc_curve.png-->
            </div>
            <div class="race_progress">
                <img src="https://michael4706.github.io/XAI_Website/img/race/loss_curve.png" style="width:100%"> <!--/img/race/loss_curve.png-->
            </div>
        </div>
        <div class = "race_acc">
                <img src="https://michael4706.github.io/XAI_Website/img/race/accuracy_barplot.png" style="width:70%"> <!--/img/race/accuracy_barplot.png-->
        </div>
        <h4><b>Biased Race Model</b>(7 classes with 38% accuracy)</h4>
         <div class="biased_race_row">
            <div class="biased_race_progress">
                <img src="https://michael4706.github.io/XAI_Website/img/biased_race/acc_curve_Brace.png" style="width:100%"> <!--/img/biased_race/acc_curve_Brace.png-->
            </div>
            <div class="biased_race_progress">
                <img src="https://michael4706.github.io/XAI_Website/img/biased_race/loss_curve_Brace.png" style="width:100%"> <!--/img/biased_race/loss_curve_Brace.png-->
            </div>
        </div>
        <div class = "biased_race_acc">
            <img src="https://michael4706.github.io/XAI_Website/img/biased_race/accuracy_barplot_Brace.png" style="width:70%"> <!--/img/biased_race/accuracy_barplot_Brac.png-->
        </div>
        <h4><b>Age Model</b>(9 classes with 55% accuracy)</h4>
        <div class = "age_row">
                <div class="age_progress">
                    <img src="https://michael4706.github.io/XAI_Website/img/age/acc_curve.png" style="width:100%"> <!--/img/age/acc_curve.png-->
                </div>
                <div class="age_progress">
                    <img src="https://michael4706.github.io/XAI_Website/img/age/loss_curve.png" style="width:100%"> <!--/img/age/loss_curve.png-->
                </div>
        </div>
        <div class = "age_acc">
                <img src="https://michael4706.github.io/XAI_Website/img/age/accuracy_barplot.png" style="width:70%"> <!--/img/age/accuracy_barplot.png-->
        </div>
        <h4><b>Gender Model</b>(2 classes with 91% accuracy)</h4>
        <div class = "gender_row">
            <div class="Gender_progress">
                <img src="https://michael4706.github.io/XAI_Website/img/gender/acc_curve.png" style="width:100%"> <!--/img/gender/acc_curve.png-->
            </div>
            <div class="Gender_progress">
                <img src="https://michael4706.github.io/XAI_Website/img/gender/loss_curve.png" style="width:100%"> <!--/img/gender/loss_curve.png-->
            </div>
        </div>
        <div class = "gender_acc">
                <img src="https://michael4706.github.io/XAI_Website/img/gender/accuracy_barplot.png" style="width:70%"> <!--/img/gender/accuracy_barplot.png-->
        </div>
    </section>
</body>