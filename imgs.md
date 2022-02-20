# LAB 12-13 - Neural Transfer Style
This work was created based on https://keras.io/examples/generative/neural_style_transfer/

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



