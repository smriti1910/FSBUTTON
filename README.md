# Ex.No: 2 To develop an application that uses GUI Components with Fonts and Colors. 
Note: Create button for colors and fonts while clicking color or font button should change 


## AIM:

To create an application that uses GUI Components with Fonts and Colors using Android Studio.

## EQUIPMENTS REQUIRED:

Latest Version Android Studio

## ALGORITHM:

Step 1: Open Android Stdio and then click on File -> New -> New project.

Step 2: Then type the Application name  and click Next.

Step 3: Then select the Minimum SDK as shown below and click Next.

Step 4: Then select the Empty Activity and click Next. Finally click Finish.

Step 5: Design layout in activity_main.xml.

Step 6: Display message give in MainActivity file.

Step 7: Save and run the application

## PROGRAM:
```
/*
Program to print the text “GUIcomponent”.
Developed by:SMRITI .B
Registeration Number :212221040156
*/
```
## activity_main.xml:
```
<?xml version="1.0" encoding="utf-8"?>
 <LinearLayout
xmlns:android="http://schemas.android.com/apk/res/android"
 android:orientation="vertical"
 android:layout_width="match_parent"
 android:layout_height="match_parent">
 <TextView
 android:id="@+id/textView"
 android:layout_width="match_parent"
 android:layout_height="wrap_content"
 android:layout_margin="30dp"
 android:gravity="center"
 android:text="STUDENT DETAILS"
 android:textSize="25sp"
 android:textStyle="bold" />
 <TextView
 android:id="@+id/textView1"
 android:layout_width="match_parent"
 android:layout_height="wrap_content"
 android:layout_margin="30dp"
 android:gravity="center"
 android:text="Name : Smriti B"
 android:textSize="15sp"
 android:textStyle="bold" />
 <TextView
 android:id="@+id/textView2"
 android:layout_width="match_parent"
 android:layout_height="wrap_content"
 android:layout_margin="30dp"
 android:gravity="center"
 android:text="Register number : 212221040156"
 android:textSize="15sp"
 android:textStyle="bold" />
 <TextView
 android:id="@+id/textView3"
 android:layout_width="match_parent"
 android:layout_height="wrap_content"
 android:layout_margin="30dp"
 android:gravity="center"
 android:text="Year : II"
 android:textSize="15sp"
 android:textStyle="bold" />
 <TextView
 android:id="@+id/textView4"
 android:layout_width="match_parent"
 android:layout_height="wrap_content"
 android:layout_margin="30dp"
 android:gravity="center"
 android:text="Dept: Computer Science and Engineering"
 android:textSize="15sp"
 android:textStyle="bold" />
 <Button
 android:id="@+id/button1"
 android:layout_width="match_parent"
 android:layout_height="wrap_content"
 android:layout_margin="20dp"
 android:gravity="center"
 android:text="Change font size"
 android:textSize="15sp" />
 <Button
 android:id="@+id/button2"
 android:layout_width="match_parent"
 android:layout_height="wrap_content"
 android:layout_margin="20dp"
 android:gravity="center"
 android:text="Change color"
 android:textSize="15sp" />
 <Button
 android:id="@+id/button3"
 android:layout_width="match_parent"
 android:layout_height="wrap_content"
 android:layout_margin="20dp"
 android:gravity="center"
 android:text="Change font style"
 android:textSize="15sp" />

 </LinearLayout>
 
 ```
 ## MainActivity.java:
 
 ```
package com.example.workshop1_156;
import android.graphics.Color;
import android.graphics.Typeface;
import android.os.Bundle;
import android.view.View;
import android.widget.Button;
import android.widget.TextView;
import androidx.appcompat.app.AppCompatActivity;
public class MainActivity extends AppCompatActivity
{
 int ch=1;
 float font=30;
 @Override
 protected void onCreate(Bundle savedInstanceState)
 {
 super.onCreate(savedInstanceState);
 setContentView(R.layout.activity_main);
 final TextView t= (TextView)
findViewById(R.id.textView);
 Button b1= (Button) findViewById(R.id.button1);
 b1.setOnClickListener(new View.OnClickListener() {
 @Override
 public void onClick(View v) {
 t.setTextSize(font);
 font = font + 5;
 if (font == 50)
 font = 30;
 }
 });
 Button b2= (Button) findViewById(R.id.button2);
 b2.setOnClickListener(new View.OnClickListener() {
 @Override
 public void onClick(View v) {
 switch (ch) {
 case 1:
 t.setTextColor(Color.RED);

 break;
 case 2:
 t.setTextColor(Color.GREEN);
 break;
 case 3:
 t.setTextColor(Color.BLUE);
 break;
 case 4:
 t.setTextColor(Color.CYAN);
 break;
 case 5:
 t.setTextColor(Color.YELLOW);
 break;
 case 6:
 t.setTextColor(Color.MAGENTA);
 break;
 }
 ch++;
 if (ch == 7)
 ch = 1;
 }
 });
 Button b3= (Button) findViewById(R.id.button3);
 b3.setOnClickListener(new View.OnClickListener() {
 @Override
 public void onClick(View v) {
 switch (ch) {
 case 1:
 t.setTypeface(null,Typeface.BOLD);
 break;
 case 2:
 t.setTypeface(null,Typeface.ITALIC);
 break;
 case 3:

t.setTypeface(null,Typeface.BOLD_ITALIC);
 break;
 case 4:
 t.setTypeface(null,Typeface.NORMAL);
 break;
 }
 ch++;
 if (ch == 5)
 ch = 1;
 }
 });
 }
}


## OUTPUT

![OUTPUT](https://github.com/smriti1910/FSBUTTON/assets/133334803/54993ec7-c8cb-4c41-9061-bb12d6cafd83)
![FONT COLOUR](https://github.com/smriti1910/FSBUTTON/assets/133334803/8f94eeba-c864-4667-a422-5c934cbe05ce)
![FONT STYLE AND SIZE](https://github.com/smriti1910/FSBUTTON/assets/133334803/a142f435-516b-4c46-8cce-86dae2a3d9b0)





## RESULT
Thus a Simple Android Application that uses GUI Components with Fonts and Colors using Android Studio is developed and executed successfully.

