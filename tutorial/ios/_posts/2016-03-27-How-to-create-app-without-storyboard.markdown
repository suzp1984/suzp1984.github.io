---
layout: content
title:  "How to create app without storyboard"
date:   2016-03-27 20:40:00 +0800
---

First Step
==========

Create the boilerplate codes from the pre-existed sample code.
The default template code is started with a storyboard, then the
next step was to delete the storyboard.

Second Step
===========

1. In the General, Delete main.storyboard in the Main interface field.
2. Delete the Main.storyboard and ViewController.swift from the project.

Third Step
==========

Create the window property in AppDelegate's init function application didFinishLaunchingWithOptions,
and set the window's rootViewController property.

```swift
    self.window = UIWindow()
    self.window!.rootViewController = UIViewController()
    self.window!.backgroundColor = UIColor.redColor()
    self.window!.makeKeyAndVisible()
    return ture
```

