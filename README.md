# dart-flutter-notes


# Starting up (i am rich app)

```void main()``` funciton is the starting point to all our fluter apps.
the first thing the app does is look inside the main function to see what what to do 

```runApp``` is a function to run wwhatever you want inside the ```void main()``` function 

# widget trees 

```materialApp``` is the parent widget  and almost all flutter apps will start of with this as the first widget 

```Text('hello world')``` is widget that allows to show text to the screen 

```Center: Text('hello world')``` is a widget that allows you to make the text appear in the center of the screen 

those are few examples of widgets that are built into  flutter 

# Scaffold 
```Scaffold``` givess you pre connfigured stuff to work with 

```
void main() {
  runApp(
    MaterialApp(
      home: Scaffold(
        appBar: AppBar(
          title: Text('I Am Rich'),
        ),
      ),
    ),
  );
}

```

with ```appBar: AppBar()``` the scaffold function gives the ability to create an app bar for our app 

this AppBar can be configurered and changed by using proprites 
i.e  ```backgroundColor``` widget
refer to material design for  more color     