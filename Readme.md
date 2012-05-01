Features
========

* UIPopoverController like working on iPhone and iPad
* Popover rendered using no images, only Quartz code
* Automatic orientation. It will find the best orientation and size for every situation
* MIT License (you can use it on your commercial apps)





What you need
---

To use FPPopoverController you only need

* FPPopoverController.m and .h    (the controller)
* FPPopoverView.m and .h
* FPTouchView.m and .m

That's it.




How to use it
---  
Let's start with a simple example
    
    -(IBAction)buttonClicked:(UIButton*)okButton
    {
        //the view controller you want to present as popover
        YourViewController *controller = [[YourViewController alloc] init]; 

        //our popover
        FPPopoverController *popover = [[FPPopoverController alloc] initWithViewController:controller]; 
        
        //the popover will be presented from the okButton view 
        [popover presentPopoverFromView:okButton]; 
    
    
        //release
        [controller release];
    }
    

