Download Link: https://assignmentchef.com/product/solved-csci5980-assignment1-camera-obscura
<br>
You will design a camera obscura with your cellphone.

In this assignment, you will design a camera obscura with your cellphone camera. The camera obscura is a dark chamber (box) with a small pinhole where light is mapped to the other side of the chamber (screen). This creates an upside-down image.

<ol>

 <li>Build a lightproof dark chamber: the chamber will be only illuminated by the light from the pinhole. Play with different size of chambers if possible. Cover the screen with a white paper and the rest of insider surfaces with black papers. Be creative!</li>

 <li>Make a pinhole on the other side of the screen. Start with a small hole (diameter<em>&lt;</em>1mm) and adjust the size of the hole to get more light. Trade-off is that the bigger hole, the brighter image but blurrier.</li>

 <li>Set the camera focal length to the manual mode (AF→MF) and adjust the focal length to see an object at the distance between the pinhole and the chamber screen.</li>

 <li>Set the camera sensitivity (<em>&gt;</em>ISO 800).</li>

 <li>Set the camera exposure time (<em>&gt;</em>8 sec).</li>

 <li>Make an additional hole where your cellphone camera can look inside. Locate your cellphone camera close to the pinhole without occluding pinhole. Make sure this hole is completely light sealed.</li>

 <li>Take a picture and adjust the pinhole size and camera settings to make better sharp image.</li>

</ol>

For an Android phone, you can control the exposure time and sensitivity easily. Camera FV-5 Lite is an app to grab a long exposure image. For iOS, the exposure control is highly limited. There are apps that simulate the long exposure effect by taking many images. This creates a noisy image. You may borrow an Android phone or old digital camera. You can also refer to the website: <a href="http://graphics.cs.cmu.edu/courses/15-463/2015_fall/hw/proj5-camera/">http://graphics.cs.cmu.edu/courses/ </a><a href="http://graphics.cs.cmu.edu/courses/15-463/2015_fall/hw/proj5-camera/">15-463/2015_fall/hw/proj5-camera/</a><a href="http://graphics.cs.cmu.edu/courses/15-463/2015_fall/hw/proj5-camera/">.</a>

Note: Lighting is extremely important. Given Minnesota’s weather, it is difficult to find a nice cloudless day. Plan outside data capture on sunny day ahead.

<strong>Write-up:</strong>

(1) Describe your design (dimension) with images and your camera setting. Share your awesome photos.

<strong>3       Where am I?</strong>

(a) Lateral view                      (b) Camera obscura image                      (c) Original image

Figure 2: You will your camera obscura to estimate depth.

Using this camera obscura, you will estimate the depth of a 3D object (from pinhole). You will take a picture containing your two friends (A and B) whom you know their height in meter where they will stand at different distance from the camera as show in Figure 2(a).

<strong>Write-up:</strong>

<ul>

 <li>Given the height of A in meter (<em>H<sub>A</sub></em>) and pixel (<em>h<sub>A</sub></em>), derive and compute the distance from A to the pinhole.</li>

 <li>Given the height of B in meter (<em>H<sub>B</sub></em>) and pixel (<em>h<sub>B</sub></em>), derive and compute the distance from B to the pinhole.</li>

</ul>

Note: You can measure pixel distance using an image viewer software, e.g., irfanview, or MATLAB.

(a) Geometry                                                                   (b) Image cropping

Figure 3: You will your camera obscura to estimate depth.

<h1>4      Dolly Zoom</h1>

You will simulate the Dolly zoom effect using your camera obscura. You will take at least two pictures with different camera locations, e.g., taking 5 step back, ∆<em>d</em>, as shown in Figure 3(a). A and B will appear smaller than the first image as ∆<em>d &gt; </em>0. You can apply the zoom-in effect by scaling and cropping the image such that A appears the same as shown in Figure 3(b). You may find a reference from here: <a href="http://www-users.cs.umn.edu/~hspark/CSci5980/Lec1_Supp_DollyZoom.pdf">http://www-users.cs.umn.edu/</a><a href="http://www-users.cs.umn.edu/~hspark/CSci5980/Lec1_Supp_DollyZoom.pdf">~</a><a href="http://www-users.cs.umn.edu/~hspark/CSci5980/Lec1_Supp_DollyZoom.pdf">hspark/CSci5980/Lec1_Supp_DollyZoom.pdf</a><a href="http://www-users.cs.umn.edu/~hspark/CSci5980/Lec1_Supp_DollyZoom.pdf">.</a>

<strong>Write-up:</strong>

<ul>

 <li>Predict the height of B in the second image given <em>h<sub>B </sub></em>in the first image. Reason about the prediction. <em>Hint: You may need to compute </em>∆<em>d with the information in the second image.</em></li>

 <li>Confirm the prediction by measuring the height of B in the second image.</li>

</ul>

Useful MATLAB functions:

<ul>

 <li><em>Load image</em>: im = imread(filename).</li>

 <li><em>Save image</em>: imwrite(im, filename).</li>

 <li><em>Resize image</em>: im = imresize(im, scale).</li>

 <li><em>Display image</em>: imshow(im) or imshow(filename).</li>

 <li><em>Measure the distance in image</em>: display the image in a figure, select the data cursor icon in the figure toolbar, and click on the image to get the coordinates of certain pixels.</li>

</ul>

Calculate the distance with the pixel coordinates.