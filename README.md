## Ex.No:1 Implementation of a Hello world Activity using all lifecycles methods using Android Studio.
## AIM:

To create Hello world Activity using all lifecycles methods to display messages using android studio.


## EQUIPMENTS REQUIRED:

Android Studio(Min. required Artic Fox)


## ALGORITHM:

Step 1: Open Android Stdio and then click on File -> New -> New project.

Step 2: Then type the Application name as HelloWorld and click Next.

Step 3: Then select the Minimum SDK as shown below and click Next.

Step 4: Then select the Empty Activity and click Next. Finally click Finish.

Step 5: Design layout in activity_main.xml.

Step 6: Display message give in MainActivity file.

Step 7: Save and run the application.


## PROGRAM:
/*
Program to implement a Hello world Activity using all lifecycles methods using Android Studio                                                                      
Developed by: ARINI A                                                                        
RegisterNumber: 212222040011
*/

## MainActivity.java:
```
package com.example.experiment_1;

import androidx.appcompat.app.AppCompatActivity;

import android.os.Bundle;
import android.widget.Toast;

public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        Toast toast=Toast.makeText(getApplicationContext(),"OnCreate Executed",Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onStart(){
        super.onStart();
        Toast toast=Toast.makeText(getApplicationContext(),"OnStart Executed",Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onResume(){
        super.onResume();
        Toast toast=Toast.makeText(getApplicationContext(),"OnResume Executed",Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onPause(){
        super.onPause();
        Toast toast=Toast.makeText(getApplicationContext(),"OnPause Executed",Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onStop(){
        super.onStop();
        Toast toast=Toast.makeText(getApplicationContext(),"OnStop Executed",Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onRestart() {
        super.onRestart();
        Toast toast = Toast.makeText(getApplicationContext(), "OnRestart Executed", Toast.LENGTH_LONG);
        toast.show();

    }
    protected void onDestroy(){
        super.onDestroy();
        Toast toast=Toast.makeText(getApplicationContext(),"OnDestroy Executed",Toast.LENGTH_LONG);
        toast.show();

    }
}
```
## activitymain.xml:
```
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">

    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Hello World!"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

</androidx.constraintlayout.widget.ConstraintLayout>
```


## OUTPUT:

## OnCreate Executed

![onCreate](https://github.com/user-attachments/assets/7fb2c505-6da6-4f67-9d10-c541b52e5a94)


## OnStart Executed 

![onStart](https://github.com/user-attachments/assets/e90579e6-7f1e-4f29-992c-cfe35f1c1679)

## OnResume Executed

![onResume](https://github.com/user-attachments/assets/30c0da7c-a0ff-4a28-864a-1dcf2a193f94)

## OnRestart Executed

![onRestart](https://github.com/user-attachments/assets/f822443b-29db-46d1-a94b-53890e4b11f1)

## onPause Executed

![onPause](https://github.com/user-attachments/assets/9925849a-ae41-49a4-bc9a-bd016fa3094b)


## RESULT:
Thus a program to implement the various life cycles of an activity is written and successfully executed using Android Studio.
