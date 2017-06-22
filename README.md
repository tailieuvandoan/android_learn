# android_learn
tự học android

- mainactivity.java
package com.example.shitoki.shitoki;

import android.support.v7.app.AppCompatActivity;
import android.os.Bundle;
import android.view.View;
import android.widget.Button;
import android.widget.TextView;

public class MainActivity extends AppCompatActivity {
    TextView txtv;
    Button btn;

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        txtv=(TextView)findViewById(R.id.abc);
        btn=(Button)findViewById(R.id.button);

        btn.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                txtv.setText("textagdvagdkhbdfjsasksyafiudyaa");
            }
        });

    }

}

- activitymain.xml
<?xml version="1.0" encoding="utf-8"?>
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
  android:background="@drawable/images"
    android:gravity="center"
    android:orientation="vertical"
    tools:context="com.example.shitoki.shitoki.MainActivity">
    <TextView
        android:id="@+id/abc"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text=""
        android:textSize="30dp"
        android:textColor="#ffff"
        />
    <Button
        android:layout_marginTop="30dp"
        android:id="@+id/button"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Button" />




</LinearLayout>
