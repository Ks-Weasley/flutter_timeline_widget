# Flutter_Timeline_Widget


A Flutter widget to list the details of upcoming bookings/events in the form of a timeline

The source code is **100% Dart**, and everything resides in the [/lib](https://github.com/gouthamkumar253/flutter_timeline_widget) folder.

## Kindly :star: the repo to support the project
 [![GitHub followers](https://img.shields.io/github/followers/gouthamkumar253.svg?style=social&label=Follow)](https://github.com/gouthamkumar253)
 [![GitHub followers](https://img.shields.io/github/followers/ks-weasley.svg?style=social&label=Follow)](https://github.com/ks-weasley)

## 💻 Installation

In the `dependencies:` section of your `pubspec.yaml`, add the following line:

```yaml
timeline_widget: <latest_version>
```

Import in your project:
```dart
import 'package:timeline_widget/timeline_widget.dart';
```

## ❔Basic Usage
```dart
import 'package:flutter/material.dart';
import 'package:ticket_pass_package/ticket_pass.dart';

void main() => runApp(MyApp());

class MyApp extends StatelessWidget {
  List<String> sample = <String>[
    'Sample data 1',
    'Sample data 2',
    'Sample data 3',
    'Sample data 4',
    'Sample data 5',
    'Sample data 6',
    'Sample data 7',
    'Sample data 8'
  ];
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      title: 'Movie Ticket Pass',
      home: Scaffold(
        appBar: AppBar(
          title: Text('Movie Ticket Pass'),
        ),
        body: Center(
          child: TicketPass(
            alignment: Alignment.center,
            animationDuration: Duration(seconds: 2),
            expansionChild: Container(
              color: Colors.black,
              height: 200,
            ),
            expandedHeight: 500,
            expandIcon: CircleAvatar(
              maxRadius: 14,
              child: Icon(
                Icons.keyboard_arrow_down,
                color: Colors.white,
                size: 20,
              ),
            ),
            expansionTitle: Text(
              'Purchased By',
              style: TextStyle(
                fontWeight: FontWeight.w600,
              ),
            ),
            purchaserList: sample,
            separatorColor: Colors.black,
            separatorHeight: 2.0,
            color: Colors.white,
            curve: Curves.easeOut,
            titleColor: Colors.blue,
            shrinkIcon: CircleAvatar(
              maxRadius: 14,
              child: Icon(
                Icons.keyboard_arrow_up,
                color: Colors.white,
                size: 20,
              ),
            ),
            ticketTitle: Text(
              'Sample title',
              style: const TextStyle(
                color: Colors.white,
                fontWeight: FontWeight.w600,
                fontSize: 18,
              ),
            ),
            titleHeight: 50,

            width: 300,
            height: 200,
            shadowColor: Colors.blue.withOpacity(0.5),
            elevation: 8,
            shouldExpand: true,
            child: Container(
              color: Colors.blue,
              width: 10,
            ),
          ),
        ),
      ),
    );
  }
}
```
## Screenshots
//![](ticket_pass.gif)

## 👨 Developed By

```
Goutham Kumar R
Krithika Swaminathan
```


