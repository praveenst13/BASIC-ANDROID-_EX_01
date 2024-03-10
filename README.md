# BASIC-ANDROID-_EX_01
## AIM:
To create a "Hello World" activity in Android that logs lifecycle events using Android Studio

## EQUIPMENTS REQUIRED:

Android Studio(Min. required Artic Fox)


## ALGORITHM:

Step 1: Open Android Stdio and Choose Start a new Android Studio project.

Step 2: Select an empty activity.

Step 3: Open MainActivity.java located in the java directory under your app's package name. Modify the file to include logging for each lifecycle method.

Step 4: Click on the "Run" button in Android Studio.

Step 5: Choose your device or emulator, then wait for the application to launch.



## PROGRAM
### DEVELOPED BY : Praveen S
### REGISTER NO: 212222240077

### MainActivity.java:
```java

package com.example.myapplication; // Make sure this matches your actual package name

import android.os.Bundle;
import android.widget.Toast;

import androidx.appcompat.app.AppCompatActivity;

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
### Activity_Main.XML:
```xml
<?xml version="1.0" encoding="utf-8"?>
<manifest xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:tools="http://schemas.android.com/tools">


    <application
        android:allowBackup="true"
        android:dataExtractionRules="@xml/data_extraction_rules"
        android:fullBackupContent="@xml/backup_rules"
        android:icon="@mipmap/ic_launcher"
        android:label="@string/app_name"
        android:roundIcon="@mipmap/ic_launcher_round"
        android:supportsRtl="true"
        android:theme="@style/Theme.MyApplication"
        tools:targetApi="31">

        <activity
            android:name=".MainActivity"
            android:exported="true">
            <intent-filter>
                <action android:name="android.intent.action.MAIN" />

                <category android:name="android.intent.category.LAUNCHER" />
            </intent-filter>
        </activity>

    </application>

</manifest>
```

## OUTPUT:
### OnCreate
![image](https://github.com/praveenst13/BASIC-ANDROID-_EX_01/assets/118787793/a33e2c87-66be-416e-918d-7a75ff1c36ed)
### OnPause
![image](https://github.com/praveenst13/BASIC-ANDROID-_EX_01/assets/118787793/660ffca8-cb93-45e3-9495-08529e4ba413)


## RESULT:
Thus a program to implement the various life cycles of an activity is written and successfully executed using Android Studio.
