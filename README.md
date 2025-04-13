import 'package:flutter/material.dart';

void main() => runApp(MyApp());

class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      home: Scaffold(
        backgroundColor: Colors.cyan, // 바깥 테두리 배경
        body: Padding(
          padding: const EdgeInsets.all(4.0),
          child: Column(
            children: [
              Expanded(
                flex: 1,
                child: Row(
                  children: [
                    Expanded(
                      flex: 3,
                      child: Container(color: Colors.red),
                    ),
                    Expanded(
                      flex: 4,
                      child: Column(
                        children: [
                          Expanded(
                            flex: 1,
                            child: Container(color: Colors.blue),
                          ),
                          Expanded(
                            flex: 1,
                            child: Row(
                              children: [
                                Expanded(
                                  flex: 1,
                                  child: Container(color: Colors.black),
                                ),
                                Expanded(
                                  flex: 1,
                                  child: Container(color: Colors.orange),
                                ),
                              ],
                            ),
                          ),
                        ],
                      ),
                    ),
                  ],
                ),
              ),
              Expanded(
                flex: 1,
                child: Container(color: Colors.yellow),
              ),
            ],
          ),
        ),
      ),
    );
  }
}
