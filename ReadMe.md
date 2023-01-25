# test for adding template mask to cv2.findTransformECC

the test is re-using the example of https://learnopencv.com/image-alignment-ecc-in-opencv-c-python/.

It sequentially run:
1. the first run is the original example.
1. The second run set a mask around the template image (red band), so the template image has less feature than the input image.
Result is degraded
1. Last run use modifications of the proposed push to use a mask around the template image within the optimization of findTransformECC. Results are then comparable to the original run.
