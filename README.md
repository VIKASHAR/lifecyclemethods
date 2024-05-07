# Ex.No:2 To create a HelloWorld Activity using all lifecycles methods to display messages.


## AIM:

To create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio.

## EQUIPMENTS REQUIRED:

Latest Version Android Studio

## ALGORITHM:

Step 1: Open Android Stdio and then click on File -> New -> New project.

Step 2: Then type the Application name as HelloWorld and click Next. 

Step 3: Then select the Minimum SDK as shown below and click Next.

Step 4: Then select the Empty Activity and click Next. Finally click Finish.

Step 5: Design layout in activity_main.xml.

Step 6: Display message give in MainActivity file.

Step 7: Save and run the application.

## PROGRAM:
```
/*
Program to print the text “Hello World”.
Developed by: Vikash.A.R
Registeration Number : 212222040179
*/
```

## In activity_main.xml
    <?xml version="1.0" encoding="utf-8"?>
    <androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
        xmlns:app="http://schemas.android.com/apk/res-auto"
        xmlns:tools="http://schemas.android.com/tools"
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        tools:context=".MainActivity">
    
        <TextView
            android:layout_width="299dp"
            android:layout_height="110dp"
            android:text="Life Cycle"
            android:textColor="#565C81"
            android:textSize="60sp"
            app:layout_constraintBottom_toTopOf="@+id/textView"
            app:layout_constraintEnd_toEndOf="parent"
            app:layout_constraintHorizontal_bias="0.633"
            app:layout_constraintStart_toStartOf="parent"
            app:layout_constraintTop_toTopOf="parent"
            app:layout_constraintVertical_bias="0.565" />
    
        <TextView
            android:id="@+id/textView"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_marginBottom="340dp"
            android:text="Hello World"
            android:textSize="24sp"
            app:layout_constraintBottom_toBottomOf="parent"
            app:layout_constraintEnd_toEndOf="parent"
            app:layout_constraintHorizontal_bias="0.468"
            app:layout_constraintStart_toStartOf="parent" />
    
    </androidx.constraintlayout.widget.ConstraintLayout>

## In MainActivity.java
    package com.example.life_cycle;
    
    import android.os.Bundle;
    import android.widget.Toast;
    
    import androidx.annotation.NonNull;
    import androidx.appcompat.app.AppCompatActivity;
    
    import com.example.life_cycle.R;
    
    public class MainActivity extends AppCompatActivity {
    
        @Override
        protected void onCreate(Bundle savedInstanceState) {
            super.onCreate(savedInstanceState);
            setContentView(R.layout.activity_main);
            Toast toast = Toast.makeText(getApplicationContext(), "onCreate Called", Toast.LENGTH_LONG);
            toast.show();
            // This method is called when the activity is first created.
        }
    
        @Override
        protected void onStart() {
            super.onStart();
            Toast toast = Toast.makeText(getApplicationContext(), "onStart", Toast.LENGTH_LONG);
            toast.show();
            // The activity is about to become visible.
        }
    
        @Override
        protected void onResume() {
            super.onResume();
            Toast toast = Toast.makeText(getApplicationContext(), "onResume", Toast.LENGTH_LONG);
            toast.show();
        }
    
        @Override
        protected void onPause() {
            super.onPause();
            Toast toast = Toast.makeText(getApplicationContext(), "onPause", Toast.LENGTH_LONG);
            toast.show();
    
        }
    
        @Override
        protected void onStop() {
            super.onStop();
            Toast toast = Toast.makeText(getApplicationContext(), "onStop", Toast.LENGTH_LONG);
            toast.show();
    
        }
    
        @Override
        protected void onDestroy() {
            super.onDestroy();
            Toast toast = Toast.makeText(getApplicationContext(), "onResume", Toast.LENGTH_LONG);
            toast.show();
    
        }
    
        @Override
        protected void onSaveInstanceState(@NonNull Bundle outState) {
            super.onSaveInstanceState(outState);
            Toast toast = Toast.makeText(getApplicationContext(), "onSave", Toast.LENGTH_LONG);
            toast.show();
    
        }
    
        @Override
        protected void onRestoreInstanceState(@NonNull Bundle savedInstanceState) {
            super.onRestoreInstanceState(savedInstanceState);
            Toast toast = Toast.makeText(getApplicationContext(), "onRestore", Toast.LENGTH_LONG);
            toast.show();
    
        }
    }



## OUTPUT
![Screenshot 2024-05-07 174415](https://github.com/VIKASHAR/lifecyclemethods/assets/119405655/345ed162-6cbc-4e1f-881d-e2490418a479)
![Screenshot 2024-05-07 174434](https://github.com/VIKASHAR/lifecyclemethods/assets/119405655/d8e87d45-b175-442c-90e6-ae2139e15319)
![Screenshot 2024-05-07 174459](https://github.com/VIKASHAR/lifecyclemethods/assets/119405655/d83b0b87-341d-48ac-998c-eff55ef5f548)
![Screenshot 2024-05-07 174515](https://github.com/VIKASHAR/lifecyclemethods/assets/119405655/a3c9cc29-6a20-4a4b-ad9c-eb996076e90b)


## RESULT
Thus a Simple Android Application create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio is developed and executed successfully.
