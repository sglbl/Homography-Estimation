# Homography-Estimation
Homography Estimation That Transforms an Image to Model Soccer Field with warpPerspective Implementation

## Model Soccer Field
![image](https://user-images.githubusercontent.com/64928475/175515210-815a1e65-5bc3-44d4-8356-580254a87935.png)

App uses model soccer field image as base image. Then estimates homography matrix and warps perspective. While warping perspective interpolates the image.
To interpolate; first uses np.linspace() to create evenly spaced sample number (dimension times).
Then uses np.meshgrid(xVector, yVector) to return coordinate matrices from coordinate vectors.
![image](https://user-images.githubusercontent.com/64928475/175516087-5613b13d-d962-4dbe-aacd-858f4db2a7cb.png)

At the end it uses scipy.interpolate.griddata() to interpolate with Nearest-neighbor interpolation method.

## Example Images
![image](https://user-images.githubusercontent.com/64928475/175515349-b38cac6b-ad10-438a-b54f-ab8ca0dae2e4.png)
![image](https://user-images.githubusercontent.com/64928475/175515408-f2aa6118-2f0c-4203-b540-8c6a7408719c.png)
