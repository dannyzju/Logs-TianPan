# notes.ios.md

Xcode, iOS SDK, Objective-C, Cocoa Touch Frameworks.

		//
		//  Supporting\ Files/main.m
		//  helloworld
		//
		//  Created by Tian Pan on 6/14/13.
		//  Copyright (c) 2013 Tian Pan. All rights reserved.
		//

		#import <UIKit/UIKit.h>

		#import "AppDelegate.h"

		int main(int argc, char *argv[])
		{
		    @autoreleasepool { // Memory Management: Automatic Reference Counting (ARC) system
		        // create an instance of the UIApplication Class
		        //                   and the app delegate (providing window/configuring before the display)
		        //     delegation is a design pattern
		        // scan Info.plist (KVs on information properties)
		        return UIApplicationMain(argc, argv, nil, NSStringFromClass([AppDelegate class]));
		    }
		}

A storyboard contains an archive of the objects, transitions, and connections that define an app’s user interface. When the app starts, MainStoryboard.storyboard is loaded and the initial view controller is instantiated from it. 

MVC

A storyboard contains scenes and segues. A scene represents a view controller, and a segue represents a transition between two scenes.

An app’s window object is not represented in the storyboard.

Use the Inspector to Examine the View Controller 右侧面板上半部分顶部有许多按钮

Add the User Interface Elements 右侧面板下半部分顶部有许多按钮

