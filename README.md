
## BASIC-ANDROID-_EX_01_Implementation of a Hello world Activity using all lifecycles methods using Android Studio.
AIM:
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
```
## PROGRAM
DEVELOPED BY : Syed Adil Basha
REGISTER NO: 212221043008
MainActivity.java:

package com.example.myfirstapp;

import android.os.Bundle;
import android.widget.Toast;

import androidx.activity.EdgeToEdge;
import androidx.appcompat.app.AppCompatActivity;
import androidx.core.graphics.Insets;
import androidx.core.view.ViewCompat;
import androidx.core.view.WindowInsetsCompat;

public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
            Toast t=Toast.makeText(getApplicationContext(),"OnCreate Called",Toast.LENGTH_SHORT);
            t.show();
    }
    protected void onStart(){
        super.onStart();
        setContentView(R.layout.activity_main);
        Toast t=Toast.makeText(getApplicationContext(),"OnStart Called",Toast.LENGTH_LONG);
        t.show();
    }
    protected void onResume(){
        super.onResume();
        setContentView(R.layout.activity_main);
        Toast t=Toast.makeText(getApplicationContext(),"OnResume Called",Toast.LENGTH_LONG);
        t.show();
    }
    protected void onRestart() {
        super.onRestart();
        setContentView(R.layout.activity_main);
        Toast t = Toast.makeText(getApplicationContext(), "OnRestart Called", Toast.LENGTH_LONG);
        t.show();
    }
    protected void onPause() {
        super.onPause();
        setContentView(R.layout.activity_main);
        Toast t = Toast.makeText(getApplicationContext(), "OnPause Called", Toast.LENGTH_LONG);
        t.show();
    }
    protected void onStop() {
        super.onStop();
        setContentView(R.layout.activity_main);
        Toast t = Toast.makeText(getApplicationContext(), "OnStop Called", Toast.LENGTH_LONG);
        t.show();
    }
    protected void onDestroy() {
        super.onDestroy();
        setContentView(R.layout.activity_main);
        Toast t = Toast.makeText(getApplicationContext(), "OnDestroy Called", Toast.LENGTH_LONG);
        t.show();
    }
}


Activity_Main.XML:

<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:id="@+id/main"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">

    <Button
        android:id="@+id/button"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Button"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.5"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.5" />

    <TextView
        android:id="@+id/textView"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Hello World!"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.453" />


</androidx.constraintlayout.widget.ConstraintLayout><?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:id="@+id/main"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">

    <Button
        android:id="@+id/button"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Button"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.5"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.5" />

    <TextView
        android:id="@+id/textView"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Hello World!"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.453" />


</androidx.constraintlayout.widget.ConstraintLayout><?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:id="@+id/main"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">

    <Button
        android:id="@+id/button"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Button"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.5"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.5" />

    <TextView
        android:id="@+id/textView"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Hello World!"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.453" />


</androidx.constraintlayout.widget.ConstraintLayout><?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:id="@+id/main"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">

    <Button
        android:id="@+id/button"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Button"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.5"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.5" />

    <TextView
        android:id="@+id/textView"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Hello World!"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.453" />


</androidx.constraintlayout.widget.ConstraintLayout>
```
## OUT PUT:
![361100658-e82eb6b0-6485-4622-bae7-b10572d73854](https://github.com/user-attachments/assets/2161da52-b214-421f-9c3e-f55bfad79fb6)
![361100689-4c5a1f98-0b11-4367-9e87-f468b9d1c091](https://github.com/user-attachments/assets/8f1d57c2-1fa3-427d-8b2e-4e410f899d13)
![361100705-c92f45a4-d542-4c8b-8f1d-6d8c3fe6c365](https://github.com/user-attachments/assets/e4498417-4901-4600-a8a2-c822899abe78)
![361100719-c7c6217f-2d02-4cd6-8aa9-04cf500126b2](https://github.com/user-attachments/assets/30108afe-a68d-4df3-b143-8989593b4c6f)


## RESULT:
Thus a program to implement the various life cycles of an activity is written and successfully executed using Android Studio.

