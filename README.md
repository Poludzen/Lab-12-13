# LAB 12-13 - Neural Transfer Style
This work was created based on https://keras.io/examples/generative/neural_style_transfer/

Main idea of this algorithms: to transfer style from one image(style image) to another(content image) with maintaining the structure of both.

In the code(ipynb document) you can see how the Neural Transfer Style algorithm works in detail: how to calculates losses, gradients, how to process images, and how to transfer styles at all. Also there are some results : with different styles and contents, with different count of layers of VGG19 neural network, with different count of iterations of transfering.

In this code two styles and two contents are presented: Styles of Pablo Picasso and Frida Kahlo, contents from Fight Club movie and Paris city view.

## Let's see how it works:

### First of all, let's define our styles

#### Pablo Picasso style : 
![alt text](https://github.com/Poludzen/Lab-12-13/blob/main/images/pablo_picasso_style.jpg?raw=true "Pablo Picasso Style")

Source : https://www.tripadvisor.ru/LocationPhotoDirectLink-g190454-d244507-i114230753-Albertina-Vienna.html

#### Frida Kahlo style: 
![alt text](https://github.com/Poludzen/Lab-12-13/blob/main/images/frida_kahlo_style.jpg?raw=true "Frida Kahlo Style")

Source : https://www.itsnicethat.com/news/taschen-frida-khalo-the-complete-paintings-publication-art-190721

### it is worth noting that these are the works of the greatest painters! So, now let's define our contents

#### Paris view content:
![alt text](https://github.com/Poludzen/Lab-12-13/blob/main/images/paris_content.jpg?raw=true "Paris content")

Source : https://paris10.ru/sites/paris10.ru/files/inline-images/eiffel-tower-2000717_1920.jpg

#### Fight Club movie screenshoot content:
![alt text](https://github.com/Poludzen/Lab-12-13/blob/main/images/fight_club_content.png?raw=true "Fight Club Content")

Source : https://hu.pinterest.com/pin/478014947922432003/?amp_client_id=CLIENT_ID(_)&mweb_unauth_id=&simplified=true

## And results of transfering!!

#### First results: On full VGG-19 Neural Network,with Picasso style on image from Fight Club
##### On 1 iteration (lead time: 33 seconds)
![alt text](https://github.com/Poludzen/Lab-12-13/blob/main/images/neural_style_0.png?raw=true "Picasso on Fight Club 1")
##### On 15 iterations(lead time: 6 minutes 8 seconds)
![alt_text](https://github.com/Poludzen/Lab-12-13/blob/main/images/neural_style_14.png?raw=true "Picasso on Fight Club 15")

#### Second result: On VGG-19 without last convolutional block in architecture,with Picasso style on image from Fight Club
##### On 1 iteration (lead time: 27 seconds)
![alt text](https://github.com/Poludzen/Lab-12-13/blob/main/images/neural_style_changed_vgg_0.png?raw=true "Picasso on FC 1, mini VGG")
##### On 15 iterations(lead time 5 minutes 12 seconds)
![alt text](https://github.com/Poludzen/Lab-12-13/blob/main/images/neural_style_changed_vgg_14.png?raw=true "Picasso on FC 15, mini VGG")
#### Conclusion: reducing the number of layers (zeroing last convolutions) leads to a loss of style transfer clarity
