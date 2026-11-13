---
layout: post
title:  "📱ZFDragableModalTransition"
date:   2014-07-07 20:29:07
categories: portfolio
platform: ios
social: ['<iframe src="https://ghbtns.com/github-btn.html?user=zoonooz&repo=ZFDragableModalTransition&type=watch&count=true" height="20" width="90" frameborder="0" scrolling="0" style="width:100px; height: 20px; margin-bottom: -6px" allowTransparency="true"></iframe>']
---

While I was working on a side project, I needed to customize the way modal view controllers are presented in iOS, with a nice animation and the ability to dismiss them interactively by dragging. So I created this library and open-sourced it on GitHub: [**ZFDragableModalTransition**](https://github.com/zoonooz/ZFDragableModalTransition).

![image](https://raw.githubusercontent.com/zoonooz/ZFDragableModalTransition/master/Screenshot/ss.gif)
{: style="text-align: center; background-color: white; border-radius: 4px; "}

You can use it like this:

```objc
- (void)prepareForSegue:(UIStoryboardSegue *)segue sender:(id)sender
{
    TaskDetailViewController *detailViewController = segue.destinationViewController;
    detailViewController.task = sender;

    // create an animator object with the modal view controller instance
    // keep a strong reference in a property so it does not get released
    self.animator = [[ZFModalTransitionAnimator alloc] initWithModalViewController:detailViewController];
    self.animator.dragable = YES;
    self.animator.direction = ZFModalTransitonDirectionBottom;
    [self.animator setContentScrollView:detailViewController.scrollview];

    // set the transitioning delegate of the modal view controller to our animator
    detailViewController.transitioningDelegate = self.animator;
    detailViewController.modalPresentationStyle = UIModalPresentationCustom;
}
```
