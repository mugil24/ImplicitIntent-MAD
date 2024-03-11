# Ex.No:3a Develop program to create a text field and a button “Navigate”. When you enter “www.gmail.com” and press navigate button it should open google page using Implicit Intents.
Program to print the text “Implicitintent”.
Developed by: vaanmugil vs
Registeration Number : 212221040174
*/


package com.example.implicitintent;

import androidx.appcompat.app.AppCompatActivity;

import android.content.Intent;
import android.net.Uri;
import android.os.Bundle;
import android.view.View;
import android.widget.Button;
import android.widget.EditText;

public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        EditText editText;
        Button button;

        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        button = findViewById(R.id.button);

        editText = (EditText) findViewById(R.id.editTextText2);


        button.setOnClickListener(new View.OnClickListener() {

            @Override

            public void onClick(View view) {

                String url=editText.getText().toString();

                Intent intent = new Intent(Intent.ACTION_VIEW, Uri.parse(url));

                startActivity(intent);

            }

        });




    }
}
```

## OUTPUT

![Screenshot (92)](https://github.com/KayyuruTharani/ImplicitIntent-MAD/assets/142209319/49e24697-42c9-4020-bcd5-55c1c1f18879)

![Screenshot (93)](https://github.com/KayyuruTharani/ImplicitIntent-MAD/assets/142209319/42f48751-384b-46c1-a0aa-da0b3200c23d)

![Screenshot (94)](https://github.com/KayyuruTharani/ImplicitIntent-MAD/assets/142209319/9ce01b24-97c8-4cad-958f-5788d99477bf)








## RESULT
Thus a Simple Android Application create a navigate button using Implicit Intent to display the gmail page using Android Studio is developed and executed successfully.
