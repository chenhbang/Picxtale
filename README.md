PicxTale
========

Steganography. Hide information inside a message. Supports hiding Venmo payment info inside image. 
Made during Hack Rice 2013.

http://hackrice.challengepost.com/submissions/20468-picxtale

## Requirements
1. Xcode 5 and iOS 7.
2. [CocoaPods](http://cocoapods.org/)

## How to run
Clone. `pod install`, open `PicxTale.xcworkspace`. RUN!

## Awesomeness
![Hidden info](https://raw.github.com/DJBen/Picxtale/master/Picxtale_demo_1.png)

![Hidden payment](https://raw.github.com/DJBen/Picxtale/master/Picxtale_demo_2.png)

## How to use
### Create photo with secret
Run and you'll see a login screen. Luckily you don't need to login so just tap `skip >>`. And you will see two example
photos which does not contain encrypted message. Tap `Grid` button on the bottom left corner and you'll see the gallery. Tap the `+` button on top right corner, you have a number of choices to add your photo. Choose one and a dialog will pop up to ask you type something to hide into the photo. Do so and you will create a photo with secret of your own!

### Reveal the secret
Choose a photo, tap `photo` -> `Reveal tale`, and you will see your secret! If a venmo payment information is included, a "payment requested" button will appear. Send this photo to your friend and he/she can pay you back within a tap.

## Use case scenario
Your friends forget to bring his/her wallet when going to restaurant with you. You could take a photo of his dish, include a [Venmo](https://venmo.com/) payment link inside and send it to him/her. Your friend pays you back within a finger tap.

You wanna give someone a surprise. Take a photo of something romantic and include **"I love you"** inside the photo. Watch her face when she's revealing the secret.

## Something glitchy
The projects has about 20 warnings. "Wut?? Are you kidding me?" No, I am talking about this seriously. **All of them are generated by my third-party libraries.** So don't worry. 

Also here's a list of existing issues:

1. The delete photo function does **not** work. 
2. Your newly added photo may not appear immediately. Please choose an arbitrary photo and tap `photo` -> `refresh` and switch back to grid view, waiting for a few seconds.
3. Sometimes when you try to `reveal` secret of the same photo more than once, the secret appears to be garbage. *I will be very appreciated if someone has any idea about this problem!*
