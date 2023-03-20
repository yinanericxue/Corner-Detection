# Corner Detection

## Context for the following equation: There's a M x M sized filter centered on (x0, y0), and we want to evaulate the intensity variation when it's shifted by (u, v) amount. This variation can measured with the following Sum of Squared Differences (SSD) equation.

<img width="722" alt="Screen Shot 2023-03-19 at 9 49 37 PM" src="https://user-images.githubusercontent.com/102645083/226249474-fb09a24b-df3e-4ebb-9e66-a17d0aa6b32e.png">

## If we have a picture like below and find the gradients of the pixels, we can also see the difference when the filter is on a plain area vs edge vs corner.

<img width="1070" alt="Screen Shot 2023-03-19 at 9 58 29 PM" src="https://user-images.githubusercontent.com/102645083/226250534-519fc735-5683-434c-b13f-41a403eccb33.png">

diagram source: https://www.cs.cmu.edu/~16385/s17/Slides/6.2_Harris_Corner_Detector.pdf

## The First Order Taylor Series Expansion for part of the equation above is:
<img width="724" alt="Screen Shot 2023-03-20 at 12 42 45 PM" src="https://user-images.githubusercontent.com/102645083/226448651-4dfcea7e-3b8a-4bca-9e6d-3467a7717663.png">

## which means:
<img width="692" alt="Screen Shot 2023-03-20 at 12 44 28 PM" src="https://user-images.githubusercontent.com/102645083/226449005-5eff7ec2-65f4-4c03-a4bd-a8f494bf1e53.png">
