# Ex.No:3a Develop program to create a text field and a button “Navigate”. When you enter “www.gmail.com” and press navigate button it should open google page using Implicit Intents.


## AIM:

To create a navigate button using Implicit Intent to display the gmail page using Android Studio.

## EQUIPMENTS REQUIRED:

Latest Version Android Studio

## ALGORITHM:

Step 1: Open Android Stdio and then click on File -> New -> New project.

Step 2: Then type the Application name as HelloWorld and click Next. 

Step 3: Then select the Minimum SDK as shown below and click Next.

Step 4: Then select the Empty Activity and click Next. Finally click Finish.

Step 5: Design layout in activity_main.xml.

Step 6: Use Intent Concept in the MainActivity file.

Step 7: Save and run the application.


## PROGRAM:
```
/*
Program to print the text “Implicitintent”.
Developed by: Vidhyasri K
Registeration Number : 212222230170
*/
```
```
package com.example.indent_app;

import android.content.Intent;
import android.net.Uri;
import android.os.Bundle;
import android.view.View;
import android.widget.Button;
import android.widget.EditText;

import androidx.appcompat.app.AppCompatActivity;

public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        EditText editText;
        Button button;

        button = findViewById(R.id.button);
        editText = findViewById(R.id.editTextText);

        button.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                String url = editText.getText().toString();
                Intent i = new Intent(Intent.ACTION_VIEW, Uri.parse(url));
                startActivity(i);
            }
        });

    }
}
```

## OUTPUT
### Design Part
<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/798ef8f7-3f30-46f0-b23b-cf040dbc5617" />

### Coding Part
<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/b06f353a-6f65-429f-9cc7-c937e45793ac" />

### App
<img width="720" height="1560" alt="image" src="https://github.com/user-attachments/assets/f6f47a95-8d6b-4de8-8150-63198aeeb1ba" />

### GMail
<img width="590" height="1280" alt="image" src="https://github.com/user-attachments/assets/74e9b3aa-4840-46a1-9504-757897f2ba12" />

## RESULT
Thus a Simple Android Application create a navigate button using Implicit Intent to display the gmail page using Android Studio is developed and executed successfully.


