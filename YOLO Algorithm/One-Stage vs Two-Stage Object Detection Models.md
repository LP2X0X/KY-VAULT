- One-stage detectors: Object classification and bounding-box regression are done directly without using pre-generated region proposals (candidate object bounding-boxes).
- Two-stage detectors: Two-stage detectors usually reach better accuracy but are slower than one-stage detectors.
	- Generation of region proposals, e.g. by selective search as in R-CNN and Fast R-CNN, or by a Region Proposal Network (RPN) as in Faster R-CNN.
	- Object classification for each region proposal. Additionally other things can be done such as bounding-box regression for refining the region proposals, binary-mask prediction etc.
![[Pasted image 20221225103231.png|center]]
