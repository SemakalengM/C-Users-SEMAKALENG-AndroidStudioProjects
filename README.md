# C-Users-SEMAKALENG-AndroidStudioProjects
package com.example.socialsparks

import android.annotation.SuppressLint
import android.os.Bundle
import android.widget.Button
import android.widget.EditText
import android.widget.Toast
import androidx.activity.enableEdgeToEdge
import androidx.appcompat.app.AppCompatActivity
import androidx.core.text.set
import androidx.core.view.ViewCompat
import androidx.core.view.WindowInsetsCompat
import com.google.android.material.textfield.TextInputLayout

class MainActivity : AppCompatActivity() {

    @SuppressLint("MissingInflatedId", "SetTextI18n")
    override fun onCreate(savedInstanceState: Bundle?) {
        super.onCreate(savedInstanceState)
        enableEdgeToEdge()
        setContentView(R.layout.activity_main)

        val resultText = findViewById<EditText>(R.id.resultText)
        val resetButton = findViewById<Button>(R.id.resetButton)
        val suggestButton = findViewById<Button>(R.id.suggestButton)

        val timeInput = findViewById<TextInputLayout>(R.id.timeInput)


        suggestButton.setOnClickListener { }
        val time = timeInput.textDirection.toString().lowercase()

        if (time.isEmpty()) {

            Toast.makeText(this, "please enter time", Toast.LENGTH_SHORT).show()

            when (time) {
                "morning" ->

                    resultText.text =
                        ("send good morning")

                when (time) {
                    "afternoon" -> {

                        resultText.text =
                            ("send good afternoon")

                        else -> {

                        }
                    }

                    else -> {
                        resultText.setText("Invalid Input")
                    }
                }
            }
            timeInput.textDirection.clear()
            resultText.text.clear()


        }
    }

    Reference: https://chatgpt.com
               https://gemini.google.com

YouTube link
https://youtube.com/@semakalengmokgwatjana?si=Oo7KQtxM4Z9MBZMZ
