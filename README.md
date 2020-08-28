# Tinify
Simple interactions with Tinify Library for EndCoronavirus. This does not shorten the usage of the API by much, but turns the basic interaction into a 1 line command.

# How To use
Clone Tinify repo into Python3x/Lib/ with ```git clone https://github.com/TrevorWinstral/Tinify.git``` and navigate into the folder and execute ```pip install -r requirements.txt```

Next you need to create and TinyPNG API key, this is very simple. Go [here](https://tinypng.com/developers) create an account and you should receive an API key.

Now move to your current project and add a file ```key.txt``` and paste the API key you have generated in there and save the file.

When you want to compress your image import the module with ```from Tinify import tiny``` and compress the image with ```tiny.compress_image(uncompressed_image=INPUT_IMAGE, compressed_image=OUTPUT_IMAGE)``` the INPUT_IMAGE and OUTPUT_IMAGE strings denoting the path of the respective images should include the extension. Here is an example using an image called home_header.jpg and I am saving the compressed image to output.jpg. This function returns True if it has run without error, otherwise it prints the error and returns False.
```
from Tinify import tiny
result = tiny.compress_image(uncompressed_image='home_header.jpg', compressed_image='out.jpg')
print(result)
```
