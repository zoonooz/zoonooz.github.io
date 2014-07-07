---
layout: post
title:  "ZFDragableModalTransition"
date:   2014-07-07 20:29:07
categories: portfolio
platform: ios
social: ['<iframe src="http://ghbtns.com/github-btn.html?user=zoonooz&repo=ZFDragableModalTransition&type=watch&count=true" height="20" width="90" frameborder="0" scrolling="0" style="width:90px; height: 20px; margin-bottom: -6px" allowTransparency="true"></iframe>']
---

While I was working on a side project, I needed to customise the way to present modal view controller in iOS to has nice animation and can be dismiss interactively by drag. So I created this repository and open source on github call [**ZFDragableModalTransition**](https://github.com/zoonooz/ZFDragableModalTransition).

<center>
![image](https://raw.githubusercontent.com/zoonooz/ZFDragableModalTransition/master/Screenshot/ss.gif)
</center>

You can use it like this

```objc
- (void)prepareForSegue:(UIStoryboardSegue *)segue sender:(id)sender
{
    TaskDetailViewController *detailViewController = segue.destinationViewController;
    detailViewController.task = sender;
    
    // create animator object with instance of modal view controller
    // we need to keep it in property with strong reference so it will not get release
    self.animator = [[ZFModalTransitionAnimator alloc] initWithModalViewController:detailViewController];
    self.animator.dragable = YES;
    self.animator.direction = ZFModalTransitonDirectionBottom;
    [self.animator setContentScrollView:detailViewController.scrollview];
    
    // set transition delegate of modal view controller to our object
    detailViewController.transitioningDelegate = self.animator;
    detailViewController.modalPresentationStyle = UIModalPresentationCustom;
}
```