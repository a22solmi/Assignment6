
# Rapport

Created a SecondActivity and added EditText and Button views. Created a SharedPreference editor and
made the button add the current text from EditText.
> String text = editText.getText().toString();  
> editor.putString("textFromSecond", text);  
> editor.apply();  

Added MainActivity to parentOf in the AndroidManifest. This gives SecondActivity a back button for
navigation back to MainActivity.

Added a button to MainActivity that starts the SecondActivity.
Added onResume() to update value of TextView when returning from SecondActivity

> SharedPreferences sharedPreferences = getSharedPreferences("textFromSecond", Context.MODE_PRIVATE);  
> String text = sharedPreferences.getString("textFromSecond", "placeholder");  
> textView.setText(text);  

![](picture1.png)
![](picture2.png)