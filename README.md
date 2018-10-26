# 16-822 Geometry-based Vision Final Project
## What we're doing here
For our final project, we will be implementing the monocular depth estimating network from "[Learning Depth from Monocular Videos using Direct Methods](http://openaccess.thecvf.com/content_cvpr_2018/papers/Wang_Learning_Depth_From_CVPR_2018_paper.pdf)" and modifying the loss function with techniques from geometry-based vision for the network to predict in dynamic environments better.

## How this is organized
 * LKVOLearner: The code from "Learning Depth from Monocular Videos using Direct Methods".  We're using this as a base to get started.
 * SfMLearner: The code that "Learning Depth from Monocular Videos using Direct Methods" uses for evaluation.  We'll probably also use this for evaluation.
 * tingvidLearner: Ting Che and David's learner.  (under construction)

## To Do:
 * Get KITTI Dataset downloaded and organized 
 * Get LKVOLeaner outputting depth predictions on KITTI
 * Evaluate depth predictions using SfMLearner
 * Recreate LKVOLeaner ourselves
 ** Yeah, yeah, we know we're just modifying the loss function, so it would save us some time by just varying the LKVOLearner's loss and not reimplementing the network.  But we really want to know how the network works and we're a bit sadistic, so here we are.
 * Modify our loss function from direct visual odometry to methods that can handle dynamic environments like [this](https://arxiv.org/pdf/1708.04398)
 * Profit 
