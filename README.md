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



# Flutter UI

```Hot Reload``` a way faster way to render changes ade in the code to the simulator 
this happens instantly rather than talking almost 30 seconds 

i.e...


```
class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      home: Scaffold(
        backgroundColor: Colors.red,
        body: Container(),
      ),
    );
  }
}

```

you can create build method by typing ```stless`` in your editir and flutter will do the rest 
then you reference ```MyApp``` inside the ```main function``` 


## Container Widget 

```container widget``` is simialr to a div in web development 
refer to flutter documintation before using a widget 

```containers```  try to be as big as possible if not giving a chilid 
when giving a child they will automatically size themselves to the  size of that child 

```SafeArea``` can be wrapped around a cointainer to make the container avoiid being placed over the notch or the camera and so on.. 

```Column``` allows you align the multiple container vertivally 
```Row``` allows you to align multiple containers Horizontally  

```Exapanded``` makes the image takes the entire space of the row or the column. if there is more then one image, then space will devided btween them equally

 ```child: Image.asset('images/dice1.png')``` this is an example of a more convineint way to imbed an image inside a container without having to call the entire ```Image()``` widget 
 ```Buttom``` is wiidget to add button .. ```FlatButton``` is an example of that and this specific widget comes with it's padding 
 when    

 ```FlatButon``` needs an ```onPressed``` paramater to actaully tell the buton what it needs to do when pressed .. this is a required proberty and not optional so whenever you have button you should alwyas tell that buton what do when pressed. 

 ```onPressed``` takes a callback function to tell that butonn what to do when pressed as shown below

 ```
 onPressed: (){
   print('left button got pressed')
 }
 ```      

 # Dart Funtions 
 as with any other programming language functions in dart are there to give your aps fucntionality 

```
void getName(){
  print('Omar Almalky')
} 
```

```stful``` class is when you want changes to accur on your code.

we use ```setState``` function if we want to make changes happen inside a state full class