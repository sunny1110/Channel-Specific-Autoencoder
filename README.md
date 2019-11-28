<h1> Channel-Specific Autoencoders </h1>

<p>An <a href= "https://en.wikipedia.org/wiki/Autoencoder"> Autoencoder </a> is an Artifical Neural Network that is trained to "encode" a given input into a specified latent space, and conversely reconstruct input from this latent space by "decoding" it. The application of such neural networks range all the way from data compression to denoising. </p>

<img src="architecture/autoencoder.png" alt="autoencoder">

<h2> Traditional Autoencoder <h2>

<p> An Autoencoder for images works in two phases. A encoding phase, where the image is "encoded" into a particular latent space size, as seen below. </p>

<img src="architecture/encoder.png">

<p> And a decoding phase, where the Neural Network "decodes" the entire image back using the latent code it was intially crunched into </p>

<img src="architecture/decoder.png">

<p> As evidenced above, the Autoencoder does this for the entire image at one go </p>

