PopupBindings

"PopupBindings" is a Cocoa sample application that demonstrates how to use the bindings to manage the contents and selection of the NSPopupButton class.  It uses the NSArrayController class to hold the data and track the selection.

This is done using the following NSPopupButton bindings:

The content binding describes the collection of objects. The collection is the objects in the array controller.

	Bind to: PopupList
	Controller Key: arrangedObjects
	Model Key Path: (leave blank)

The contentValues binding describes what will be displayed in the pop-up menu. In this example it will be "name" portion of the Person object. Use the following choices for the contentValues binding:

	Bind to: PopupList
	Controller Key: arrangedObjects
	Model Key Path: name

The selectedIndex binding describes the indexed selection the user chose from the menu. Use the following choices for the selectedIndex binding:

	Bind to: PopupList
	Controller Key: selectionIndex
	Model Key Path: (leave blank)

All four NSTextFields describing the person's address is bound to the array controller's selection using a specific NSDictionary key.  So for the "street" NSTextField, its value binding should look like:

	Bind to: PopupList
	Controller Key: selection
	Model Key Path: addressStreet


Sample Requirements
The supplied Xcode project builds with Mac OS X 10.6 and runs on 10.5.x or later.


Changes from Previous Versions
n/a


Packaging List
AppDelegate.m
AppDelegate.h
	NSApp's main delegate, manages MyWindowController and helps open the sample's ReadMe from the Help menu.

MyWindowController.h
MyWindowController.m
	The NSWindowController object for the sample's main window.


Feedback and Bug Reports
Please send all feedback about this sample by connecting to the Contact ADC page.
Please submit any bug reports about this sample to the Bug Reporting page.


Developer Technical Support
The Apple Developer Connection Developer Technical Support (DTS) team is made up of highly qualified engineers with development expertise in key Apple technologies. Whether you need direct one-on-one support troubleshooting issues, hands-on assistance to accelerate a project, or helpful guidance to the right documentation and sample code, Apple engineers are ready to help you.  Refer to the Apple Developer Technical Support page.

Copyright © 2009 Apple Inc. All rights reserved.