<h1> Channel-Specific Autoencoders </h1>

<p>An <a href= "https://en.wikipedia.org/wiki/Autoencoder"> Autoencoder </a> is an Artifical Neural Network that is trained to "encode" a given input into a specified latent space, and conversely reconstruct input from this latent space by "decoding" it. The application of such neural networks range all the way from data compression to denoising. </p>

<img src="architecture/autoencoder.png" alt="autoencoder">
<br/>

<h2>Traditional Autoencoder</h2>

<p> An Autoencoder for images works in two phases. A encoding phase, where the image is "encoded" into a particular latent space size, as shown for a 32x32x3 image below: </p><br/>
<p align="center">
<img src="architecture/encoder.png" height="25%" width="25%">
</p>

<p> And a decoding phase, where the Neural Network "decodes" the entire image back using the latent code it was intially crunched into, as seen below:</p><br/>
<p align="center">
<img src="architecture/decoder.png" height="25%" width="25%" align="center">
</p>
<p> As evidenced above, the entire image is fed into the Autoencoder at one go, to encoder and decode from a single latent space.</p>


<h2> Channel-Specific-Autoencoder </h2>

<p> My design of a Channel-Specific-Autoencoder involves splitting the image into seperate colour channels of R, G, and B and feeding them to three seperate encoders to encoder into separate latent-spaces and decode the individual channels from seperately, and stack together to reconstruct the entire image. A depiction of it can be seen below: </p>

<p align="center">
  <img src="architecture/csae.png>
</p>
  
