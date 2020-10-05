# Pixel Operations and Intensity Transformations

Images get degraded through various processes. How do you enhance the visual quality of degraded images using various point intensity transformations?

![use](https://media.giphy.com/media/H5QuTLeUZUwMne6iGz/giphy.gif)

## How to use:
1. Install conan: https://docs.conan.io/en/latest/installation.html
2. Clone this repo with zip.
3. `cd imgui-opencv\` // go to the location of this project
4. `conan install (location of the project) build` **
5. `conan build  (location of project)`
6. `.\bin\imgui-opencv`
7. Click 'Open' to open the image

** If you are having issues with install part what you may need to use is `conan install (location of the project) --build=missing` this will take a while but will help get you to where you can run the project. do this if your are getting any errors when trying `conan install` step

## Testing the program
Please visit the test_image_urls.txt file for a list of urls you can use for testing.
### Objective: GIVEN an image, THEN enable "Image Negative".
```sh
Select "Image Negative" and click "Apply"
```
Test Result: "Image Negative" applied
### Objective: GIVEN a bad URL, THEN log an error message.
```sh
Paste "https://raw.githubusercontent.com/cleverSheep/ecu_flood/master/app/another_dark.jp" into the URL input and click "Apply"
```
Test Result: HTTP Exception: Not Found: https://raw.githubusercontent.com/cleverSheep/ecu_flood/master/app/another_dark.jp

## Tips
When applying the "Power Law Gamma" effect, make sure to enter the appropriate values in your terminal after you click apply.

## Contributors
* Dean Murray
* Carlos Zoido
* Austin Pickard
