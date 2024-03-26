# CS-450
### Project 1: Edge Detection (colab)
- using different algorithms like Laplacian Filter and Hough Transform to detect and locate circles of different sizes in a busy image.
  
![image](https://github.com/brayway05/Project-Links/assets/61756717/c83aee94-8a26-4be7-b4ed-719b8e2be377)
<img width="435" alt="Screenshot 2024-03-25 at 7 54 32 PM" src="https://github.com/brayway05/Project-Links/assets/61756717/0a4dd449-96fe-459d-9324-ff3700495bfc">

^ Edge Detection on image

<img width="425" alt="Screenshot 2024-03-25 at 7 54 47 PM" src="https://github.com/brayway05/Project-Links/assets/61756717/2b881716-817a-490d-8569-4a9d1411540f">

^ Hough Transform Algorithm

<img width="423" alt="Screenshot 2024-03-25 at 7 55 00 PM" src="https://github.com/brayway05/Project-Links/assets/61756717/0994653b-3727-4fb1-a5c0-9474ab6d6129">

^ Detected Cirlces with specified radius
   
### Project 2: Graph Cut Segmentation (VS-code)
- using pymaxflow to turn an image into a graph for 2-part segmentation.
- use boundary and region terms for source and sink nodes of the graph.
- use probability density functions and negative log-likelihood for edge weight calculation.

<img width="982" alt="Screenshot 2024-03-25 at 7 55 20 PM" src="https://github.com/brayway05/Project-Links/assets/61756717/ad4fcb0f-77ae-46c4-b2ed-2cd6d63cef9d">
<img width="979" alt="Screenshot 2024-03-25 at 7 55 37 PM" src="https://github.com/brayway05/Project-Links/assets/61756717/57a112dc-92b2-4d87-9952-be35897abb15">

### Project 3: Panoramic Mosaicing (VS-code)
- using SIFT algorithm for corner detectign and feature descriptor matching (opencv).
- calculating homography (linear transformation) to stitch images together where the pairs of matches are located on the images.
- finding best homographies by implementing the RANSAC algorithm.
- stiching images manually using translation matrices taken from the homographies themselves and extracting the changes in x and y of the warped image.

<img width="1005" alt="Screenshot 2024-03-25 at 7 55 53 PM" src="https://github.com/brayway05/Project-Links/assets/61756717/1c7f92e6-836f-4671-b946-c4b3320f64ad">

^ Original images

<img width="783" alt="Screenshot 2024-03-25 at 7 56 06 PM" src="https://github.com/brayway05/Project-Links/assets/61756717/defad538-ca4e-4995-b514-a16b00dcef20">

^ SIFT descriptors

<img width="495" alt="Screenshot 2024-03-25 at 7 57 01 PM" src="https://github.com/brayway05/Project-Links/assets/61756717/45c3263c-b27a-4154-9b13-65f3163bc9e6">

^ Matched descriptors

<img width="514" alt="Screenshot 2024-03-25 at 5 37 17 PM" src="https://github.com/brayway05/CS-450/assets/61756717/16f49713-03a7-4e8f-932d-cfe23c856a40">

^ Final result: Post Homography and transformation with cropping and blurring

### Project 4: QR-code reader (VS-code)
- scan horizontall and vertically on numpy image looking for a 1:1:3:1:1 ratio to find the centers of the 3 corners.
- with the 3 coordinates for the corners, find homography to rotate the QR code to an upright position for easy discretization and decoding.
- discretize given a set of possible QR code sizes (using timing information encoded into QR code).
- decode the QR code.

<img width="178" alt="Screenshot 2024-03-25 at 7 57 18 PM" src="https://github.com/brayway05/Project-Links/assets/61756717/99c5a9a8-a516-43e5-94fb-1c3d5c5b614d">
<img width="205" alt="Screenshot 2024-03-25 at 7 57 30 PM" src="https://github.com/brayway05/Project-Links/assets/61756717/4f1e1ab5-c876-4c64-815f-95274a508d49">

^ Original QR code photos
  
<img width="378" alt="Screenshot 2024-03-25 at 7 57 46 PM" src="https://github.com/brayway05/Project-Links/assets/61756717/c41acff1-67e7-4d3e-92c5-5d4f3cb5b642">
<img width="379" alt="Screenshot 2024-03-25 at 7 57 58 PM" src="https://github.com/brayway05/Project-Links/assets/61756717/44e83817-1d66-44c4-ba4e-36ed8bc3d2ae">

^ Finding 3 corners

<img width="369" alt="Screenshot 2024-03-25 at 7 58 09 PM" src="https://github.com/brayway05/Project-Links/assets/61756717/adb7ec6d-4351-4228-96e0-c903719f3c4d">
<img width="367" alt="Screenshot 2024-03-25 at 7 58 21 PM" src="https://github.com/brayway05/Project-Links/assets/61756717/2e9fb44c-fd70-4add-88ed-9deda200070b">

^ Final result before decoding: Finding 4th corner and computed homography

`Decoded QR code 1: http://byu.edu`
`Decoded QR code 2: http://byu.edu`

### Project 5: Deep-Learning Object Recognition
