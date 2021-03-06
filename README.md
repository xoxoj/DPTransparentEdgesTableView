DPTransparentEdgesTableView (Swift and Objective-C implementation)
=================================

Table and scroll view with transparent top and bottom edges. Written in Objective-C and Swift

![BackgroundImage](https://raw.githubusercontent.com/denisprokopchuk/DPTransparentEdgesTableView-Swift/master/Screenshot.png)

###Easy to use

Objectve-C
```
// Create instance of DPTransparentEdgesTableView or DPTransparentEdgesScrollView
DPTransparentEdgesTableView *tableView = [[DPTransparentEdgesTableView alloc] initWithFrame:CGRectMake(0, 20, self.view.frame.size.width, self.view.frame.size.height - 20) style:UITableViewStyleGrouped];

// Set factor that describe length of the gradient
// length = viewHeight * gradientFactor
tableView.gradientLengthFactor = 0.3;

// Start use table
tableView.delegate = self;
tableView.dataSource = self;
[self.view addSubview:tableView];
```

Swift
```swift

// Create instance of DPTransparentEdgesTableView or DPTransparentEdgesScrollView
let tableView = DPTransparentEdgesTableView(frame: CGRectMake(0, 20, view.frame.size.width, view.frame.size.height - 20))

// Set factor that describe length of the gradient
// length = viewHeight * gradientFactor
tableView.gradientLengthFactor = 0.3

// Start use table
tableView.delegate = self
tableView.dataSource = self
view.addSubview(tableView)
```

### Installation

DPTransparentEdgesTableView is available through [CocoaPods](http://cocoapods.org).

To install add the following line to your Podfile:

    pod 'DPTransparentEdgesTableView'
