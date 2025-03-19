# MobileAPP_Pertemuan2
Projeck pertemuan 2
import 'package:flutter/material.dart';

void main() {
  runApp(MyApp());
}

class MyApp extends StatelessWidget {
  const MyApp();

  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      title: 'flutter demo',
      theme: ThemeData(
        primaryColor: Colors.blue,
        primarySwatch: Colors.blue,
        appBarTheme: const AppBarTheme(backgroundColor: Colors.blue),
      ),
      home: RumahSaya(),
      debugShowCheckedModeBanner: false,
    );
  }
}

class RumahSaya extends StatelessWidget {
  const RumahSaya();

  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(title: Text('Contohnya')),
      body: Center(
        child: Column(
          mainAxisAlignment: MainAxisAlignment.center,
          children: <Widget>[
            Text("Keren CUY"),
            Container(
              height: 100,
              width: 100,
              color: Colors.blue,
              child: Text('Keren CUY'),
            ),
            Row(
              mainAxisAlignment: MainAxisAlignment.center,
              children: <Widget>[
                Container(
                  height: 100,
                  width: 100,
                  color: Colors.blue,
                  child: Text('Keren CUY'),
                ),
                Container(
                  height: 100,
                  width: 100,
                  color: Colors.red,
                  child: Text('Keren CUY'),
                ),
              ],
            ),
            Icon(Icons.home, color: Colors.blue),
            Image.network(""),
          ],
        ),
      ),
    );
  }
}
