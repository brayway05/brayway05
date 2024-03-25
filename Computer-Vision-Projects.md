# CS-450
### Project 1: Edge Detection (colab)
- using different algorithms like Laplacian Filter and Hough Transform to detect and locate circles of different sizes in a busy image.
  
<img width="737" alt="Screenshot 2024-03-25 at 5 27 53 PM" src="https://github.com/brayway05/CS-450/assets/61756717/9105fa20-3836-475b-857f-9ccc13c80ee0">
<img width="437" alt="Screenshot 2024-03-25 at 5 29 14 PM" src="https://github.com/brayway05/CS-450/assets/61756717/02773416-4e28-4044-a297-7ea9dbcbfe34">

^ Edge Detection on image

<img width="430" alt="Screenshot 2024-03-25 at 5 29 39 PM" src="https://github.com/brayway05/CS-450/assets/61756717/3a9e4ec3-ce93-4575-b673-9e92a3d01ef3">

^ Hough Transform Algorithm

<img width="433" alt="Screenshot 2024-03-25 at 5 30 11 PM" src="https://github.com/brayway05/CS-450/assets/61756717/61ae6412-a3ea-4277-9a99-bf3272596833">

^ Detected Cirlces with specified radius
   
### Project 2: Graph Cut Segmentation (VS-code)
- using pymaxflow to turn an image into a graph for 2-part segmentation.
- use boundary and region terms for source and sink nodes of the graph.
- use probability density functions and negative log-likelihood for edge weight calculation.

<img width="985" alt="Screenshot 2024-03-25 at 5 34 06 PM" src="https://github.com/brayway05/CS-450/assets/61756717/e47095bf-2acf-41c9-a1f2-1ddbfcd09b1e">
<img width="984" alt="Screenshot 2024-03-25 at 5 34 28 PM" src="https://github.com/brayway05/CS-450/assets/61756717/8bfabc17-92d7-489e-8284-1fbde4742715">


### Project 3: Panoramic Mosaicing (VS-code)
- using SIFT algorithm for corner detectign and feature descriptor matching (opencv).
- calculating homography (linear transformation) to stitch images together where the pairs of matches are located on the images.
- finding best homographies by implementing the RANSAC algorithm.
- stiching images manually using translation matrices taken from the homographies themselves and extracting the changes in x and y of the warped image.

<img width="1361" alt="Screenshot 2024-03-25 at 5 35 53 PM" src="https://github.com/brayway05/CS-450/assets/61756717/a71d53b8-de94-44c3-bbca-dee23c547eb3">

^ Original images

<img width="787" alt="Screenshot 2024-03-25 at 5 36 33 PM" src="https://github.com/brayway05/CS-450/assets/61756717/56da11e0-fb99-483b-99a8-67c354537852">

^ SIFT descriptors

<img width="553" alt="Screenshot 2024-03-25 at 5 36 54 PM" src="https://github.com/brayway05/CS-450/assets/61756717/965a44b9-4186-40bc-a87e-24939e43e04e">

^ Matched descriptors

<img width="514" alt="Screenshot 2024-03-25 at 5 37 17 PM" src="https://github.com/brayway05/CS-450/assets/61756717/16f49713-03a7-4e8f-932d-cfe23c856a40">

^ Final result: Post Homography and transformation with cropping and blurring

### Project 4: QR-code reader (VS-code)
- scan horizontall and vertically on numpy image looking for a 1:1:3:1:1 ratio to find the centers of the 3 corners.
- with the 3 coordinates for the corners, find homography to rotate the QR code to an upright position for easy discretization and decoding.
- discretize given a set of possible QR code sizes (using timing information encoded into QR code).
- decode the QR code.

<img width="201" alt="Screenshot 2024-03-25 at 5 41 04 PM" src="https://github.com/brayway05/CS-450/assets/61756717/956fa2b2-e09b-4ad7-a2c4-e7ce5b9db311">
<img width="231" alt="Screenshot 2024-03-25 at 5 41 14 PM" src="https://github.com/brayway05/CS-450/assets/61756717/95cc54de-4a6a-463c-a451-06601bc99eab">

^ Original QR code photos
  
<img width="420" alt="Screenshot 2024-03-25 at 5 38 51 PM" src="https://github.com/brayway05/CS-450/assets/61756717/70c81737-20de-4461-b84f-abdd2aefaabe">
<img width="425" alt="Screenshot 2024-03-25 at 5 39 11 PM" src="https://github.com/brayway05/CS-450/assets/61756717/d698c737-1b8e-425e-b802-7b22529ab8d0">

^ Finding 3 corners

<img width="409" alt="Screenshot 2024-03-25 at 5 39 48 PM" src="https://github.com/brayway05/CS-450/assets/61756717/d544e7ff-3590-4590-85cc-345a8ecd6890">
<img width="425" alt="Screenshot 2024-03-25 at 5 40 44 PM" src="https://github.com/brayway05/CS-450/assets/61756717/76cc1c1e-a7f6-421e-8a8c-8de706c98bad">

^ Final result before decoding: Finding 4th corner and computed homography

`Decoded QR code 1: http://byu.edu`
`Decoded QR code 2: http://byu.edu`

### Project 5: Deep-Learning Object Recognition
