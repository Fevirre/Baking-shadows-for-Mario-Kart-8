# Baking-shadows-for-Mario-Kart-8
Now that you made your track in roblox studio you want to know how to bake shadows onto your track and that's what we are going to learn today, for this example im going
to use the tour model of GBA Sunset Wilds so follow along

Go ahead and open up blender and click the shading tab on the top screen and then move to which part of your track you want to apply shadows to
you also need to move over to viewpoint shading, you'll see in a minute
![Screenshot (149)](https://user-images.githubusercontent.com/77900806/185668732-96bd8860-9363-42f7-b959-fa13a385186b.png)

Now you then want to move over to add>light>sun 
move the sun above your model and go ahead and move over to render properties and switch the render engine from Eevee to Cycles, this will cast sun position shadows
![Screenshot (150)](https://user-images.githubusercontent.com/77900806/185670726-71cee66e-833e-44bd-8a2a-988e25b8d7b2.png)

Now that we are in cycles render, the render will appear pixelated
go ahead and start dragging a yellow icon under the sun and drag it to a position to your liking
![Screenshot (152)](https://user-images.githubusercontent.com/77900806/185671663-aadec60c-b7ea-462f-a47d-8c1ebf7d403c.png)

Now that is done the road is using a material already applied from roblox studio such as MeshPart.001, we want to remove that and add a new material
![Screenshot (153)](https://user-images.githubusercontent.com/77900806/185672536-6469eac7-b9b7-413c-b0bf-3bdb74888df0.png)

now that's been replaced you want to click on your part and move to edit mode and make sure every part of your road is inside the square
also go to UV editing to make sure it's being applied
![Screenshot (154)](https://user-images.githubusercontent.com/77900806/185673568-06b71278-03cf-45ee-acb8-54bd1f29d6a2.png)

Before we start adding in the shadows, you need to make sure the part you selected has a 2nd UV layer as shown here
![Screenshot (156)](https://user-images.githubusercontent.com/77900806/185674976-28505714-d14d-4077-a20c-33994f7f32de.png)

Now that the 2nd UV layer is in, move down to here this is where you will add in the texture for the shadows to appear
press Shift+A and then add in Texture and then click on Image Texture, name your texture to something like Road since we have selected the road
MAKE SURE YOUR UV LAYER IS SELECTED!!
![Screenshot (157)](https://user-images.githubusercontent.com/77900806/185676768-e5aa0d41-6ca0-4c1e-bff7-dd2214bce4a4.png)

Go back to edit mode and then go to render properties, go down to bake and then click on the following setting
![Screenshot (160)](https://user-images.githubusercontent.com/77900806/185678150-cc33beb0-b457-4df9-9ca5-1a982bc4f12c.png)

Now you should get a result like this and then save the image as, this is the trackAO texture. do the same for shadows but this time clicking on shadows and then bake
and then save the image as
![Screenshot (161)](https://user-images.githubusercontent.com/77900806/185678605-aa27c4b4-2427-47c5-9d40-2a85dbd8ef88.png)
![Screenshot (162)](https://user-images.githubusercontent.com/77900806/185679035-b2aad573-7760-4abd-b5df-0fc61089acc2.png)

Now for the channel editing part, you can use any photo editing software that has channel editing but for this i'll be using photopea
you'll also need a background layer for this, here take it![Layer](https://user-images.githubusercontent.com/77900806/185679906-36833cb3-490e-4dca-baf4-836676758279.png)

This red image will be used for the RGB channel
go ahead and go to photopea and open from computer the red layer and then drag and drop your AO and Shadow textures onto the layer section
![Screenshot (163)](https://user-images.githubusercontent.com/77900806/185682273-257147f6-20bf-4e27-9860-3ea5b6bc6caa.png)

Make sure you add an alpha channel first and then press ctrl i 
![Screenshot (164)](https://user-images.githubusercontent.com/77900806/185683443-f01bfe8f-1aa9-442a-b8ed-b85d228b28fe.png)
![Screenshot (165)](https://user-images.githubusercontent.com/77900806/185683506-b869b39e-d09b-44e7-8ec2-5fb7d7197595.png)



Select the red channel and go to image and apply image, select the AO texture
for the green channel go to image and apply image and then select the shadow texture
![Screenshot (168)](https://user-images.githubusercontent.com/77900806/185683647-7fec4701-c73f-4edc-bb2c-8f1354d2e7cc.png)

Go ahead and go to file and then export as png, name it to whatever suits you and then go to track studio

