I had trouble getting COCO format .json predictions from the models. It seems like this is natively supported in the code, but I wasn't able to find documentation of the correct parameters to add to the config file to make it work. 

This repo has the files I edited as a workaround. 
https://github.com/yrrah/models/commit/0574a89abd80964fa5a7ed6dd00fcf211b4c2d52

The edits to inputs.py are particularly hacky. I replace the hashed image ids with the actual image ids extracted from the image filenames. I'd just change the comments to test a model on a different dataset. 
