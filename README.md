# Multiple-screens-layout
signup.xml:

<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android" xmlns:app="http://schemas.android.com/apk/res-auto"
 xmlns:tools="http://schemas.android.com/tools" 
android:layout_width="match_parent" 
android:layout_height="match_parent" 
android:padding="16dp" 
tools:context=".signup_page">
 <TextView
 android:id="@+id/create_account_text" 
android:layout_width="wrap_content"
 android:layout_height="wrap_content"
 android:text="Create Account"
 android:textSize="32sp"
 android:textStyle="bold" 
android:textColor="#3F51B5" 
app:layout_constraintTop_toTopOf="parent"
 app:layout_constraintStart_toStartOf="parent"
 app:layout_constraintEnd_toEndOf="parent"
 android:layout_marginTop="32dp" /> 
<TextView
 android:id="@+id/text_create"
 android:layout_width="wrap_content" 
android:layout_height="wrap_content"
 android:text="Enter your details to make a new account" 
android:textColor="@android:color/black"
 android:textSize="16sp" 
app:layout_constraintTop_toBottomOf="@id/create_account_text" app:layout_constraintStart_toStartOf="parent" 
app:layout_constraintEnd_toEndOf="parent"
 android:layout_marginTop="8dp" /> 
<EditText 
android:id="@+id/name" 
android:layout_width="0dp"
 android:layout_height="50dp"
 android:layout_marginHorizontal="16dp"
 android:layout_marginTop="308dp" 
android:background="@android:drawable/edit_text"
 android:hint="Username"
 android:inputType="text" 
android:padding="12dp" 
android:textColor="#000000"
 android:textColorHint="#757575" 
app:layout_constraintEnd_toEndOf="parent"
 app:layout_constraintStart_toStartOf="parent"
 app:layout_constraintTop_toBottomOf="@id/text_create" />

 <EditText
 android:id="@+id/email" 
android:layout_width="0dp"
 android:layout_height="50dp" 
android:layout_marginHorizontal="16dp"
 android:background="@android:drawable/edit_text" 
android:hint="Email" 
android:inputType="textEmailAddress"
 android:padding="12dp"
 android:textColor="#000000"
 android:textColorHint="#757575" 
app:layout_constraintEnd_toEndOf="parent" 
app:layout_constraintStart_toStartOf="parent" 
tools:layout_editor_absoluteY="168dp" />

 <EditText 
android:id="@+id/password1"
 android:layout_width="0dp"
 android:layout_height="50dp"
 android:layout_marginHorizontal="16dp" 
android:layout_marginTop="36dp" 
android:background="@android:drawable/edit_text"
 android:hint="Password" 
android:inputType="textPassword" 
android:padding="12dp" 
android:textColor="#000000" 
android:textColorHint="#757575" 
app:layout_constraintEnd_toEndOf="parent" 
app:layout_constraintHorizontal_bias="0.0" 
app:layout_constraintStart_toStartOf="parent" 
app:layout_constraintTop_toBottomOf="@id/email" />
 
<EditText 
android:id="@+id/password2" 
android:layout_width="0dp" 
android:layout_height="50dp" 
android:layout_marginHorizontal="16dp" 
android:layout_marginTop="28dp" 
android:background="@android:drawable/edit_text" 
android:hint="Confirm Password" 
android:inputType="textPassword" 
android:padding="12dp" 
android:textColor="#000000" 
android:textColorHint="#757575" 
app:layout_constraintEnd_toEndOf="parent" 
app:layout_constraintHorizontal_bias="0.0" 
app:layout_constraintStart_toStartOf="parent" 
app:layout_constraintTop_toBottomOf="@id/password1" />
 
<Button 
android:id="@+id/signup" 
android:layout_width="0dp" 
android:layout_height="wrap_content" 
android:layout_marginHorizontal="32dp" 
android:layout_marginTop="112dp" 
android:backgroundTint="#3F51B5" 
android:text="Sign Up" 
android:textColor="@android:color/white" 
android:textSize="18sp" 
app:layout_constraintEnd_toEndOf="parent" 
app:layout_constraintStart_toStartOf="parent" 
app:layout_constraintTop_toBottomOf="@id/password2" />
 
<TextView 
android:id="@+id/have_acc" 
android:layout_width="wrap_content" 
android:layout_height="wrap_content" 
android:text="Already have an account? LOG IN" 
android:textColor="#F44336" 
android:textSize="14sp" 
android:textStyle="bold" 
app:layout_constraintTop_toBottomOf="@id/signup" 
app:layout_constraintStart_toStartOf="parent" 
app:layout_constraintEnd_toEndOf="parent" 
android:layout_marginTop="16dp" />

 <TextView 
android:id="@+id/continue_with" 
android:layout_width="wrap_content"
 android:layout_height="wrap_content" 
android:text="Or continue with"
 android:textColor="#3F51B5" 
android:textStyle="bold" 
android:textSize="16sp"
 app:layout_constraintTop_toBottomOf="@id/have_acc"
 app:layout_constraintStart_toStartOf="parent"
 app:layout_constraintEnd_toEndOf="parent"
 android:layout_marginTop="32dp" />

 <LinearLayout
 android:layout_width="wrap_content"
 android:layout_height="wrap_content" 
android:layout_marginTop="168dp" 
android:gravity="center"
 android:orientation="horizontal"
 app:layout_constraintEnd_toEndOf="parent" 
app:layout_constraintHorizontal_bias="0.625"
 app:layout_constraintStart_toStartOf="parent" app:layout_constraintTop_toBottomOf="@id/continue_with">

 <ImageButton 
android:id="@+id/facebookButton"
 android:layout_width="40dp"
 android:layout_height="40dp" 
android:layout_margin="8dp"
 android:background="@null" 
android:contentDescription="Facebook Login"
 android:src="@drawable/fb" /> 

<ImageButton 
android:id="@+id/googleButton"
 android:layout_width="40dp" 
android:layout_height="40dp"
 android:layout_margin="8dp"
 android:background="@null"
 android:contentDescription="Google Login" 
android:src="@drawable/google" /> 

<ImageButton 
android:id="@+id/appleButton"
 android:layout_width="40dp" 
android:layout_height="40dp" 
android:layout_margin="8dp"
 android:background="@null" 
android:contentDescription="Apple Login"
 android:src="@drawable/apple" />

 <ImageButton 
android:id="@+id/twitterButton"
 android:layout_width="40dp"
 android:layout_height="40dp" 
android:layout_margin="8dp"
 android:background="@null" 
android:contentDescription="Twitter Login" 
android:src="@drawable/twitter" /> 

</LinearLayout>
</androidx.constraintlayout.widget.ConstraintLayout>

signup.java:
package com.example.haris_assignment2;
import android.content.Intent;
import android.os.Bundle;
import android.view.View;
import androidx.activity.EdgeToEdge;
import androidx.appcompat.app.AppCompatActivity;
import androidx.core.graphics.Insets;
import androidx.core.view.ViewCompat;
import androidx.core.view.WindowInsetsCompat;

public class signup_page extends AppCompatActivity {
 public void backtologin(View view){ 
Intent intent = new Intent(this, MainActivity.class); 
startActivity(intent); 
}
 public void backtologin2(View v){ 
Intent i = new Intent(this, MainActivity.class);
 startActivity(i);
 }
 @Override 
protected void onCreate(Bundle savedInstanceState) {
 super.onCreate(savedInstanceState); 
EdgeToEdge.enable(this);
 setContentView(R.layout.activity_signup_page); 

ViewCompat.setOnApplyWindowInsetsListener(findViewById(R.id.main), (v, insets) -> 
{
 Insets systemBars = insets.getInsets(WindowInsetsCompat.Type.systemBars()); v.setPadding(systemBars.left, systemBars.top, systemBars.right, systemBars.bottom); 
return insets; 
});
 }
}


login.xml:
<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android" xmlns:app="http://schemas.android.com/apk/res-auto"
 xmlns:tools="http://schemas.android.com/tools"
 android:id="@+id/main"
 android:layout_width="match_parent" 
android:layout_height="match_parent"
 tools:context=".MainActivity"> 
<TextView 
android:id="@+id/login_text" 
android:layout_width="wrap_content" 
android:layout_height="wrap_content" 
android:layout_centerHorizontal="true" 
android:layout_marginTop="50dp"
 android:layout_marginBottom="10dp"
 android:text="Login Page" 
android:textColor="#3F51B5"
 android:textSize="50dp" 
android:textStyle="bold" />
 <TextView 
android:id="@+id/welcome" 
android:layout_width="wrap_content" 
android:layout_height="wrap_content" 
android:layout_below="@+id/login_text" 
android:layout_centerHorizontal="true" 
android:text="Welcome Back" 
android:textColor="@color/black" 
android:textSize="20dp" 
android:textStyle="bold" />

 <EditText
 android:id="@+id/email_edit"
 android:layout_width="match_parent" 
android:layout_height="50dp" 
android:layout_below="@id/welcome" 
android:layout_marginHorizontal="20dp" 
android:layout_marginTop="40dp" 
android:background="@drawable/edittext_styling" 
android:drawablePadding="4dp" 
android:hint="Email" 
android:inputType="textEmailAddress" 
android:padding="8dp" 
android:textColor="#000000" 
android:textColorHint="#4B4343" /> 

<EditText
 android:id="@+id/password" 
android:layout_width="match_parent" 
android:layout_height="50dp" 
android:layout_below="@id/email_edit" 
android:layout_marginHorizontal="20dp"
 android:layout_marginTop="32dp" 
android:background="@drawable/edittext_styling" 
android:drawablePadding="4dp" 
android:hint="Password" 
android:inputType="textPassword" 
android:padding="8dp"
 android:textColor="#000000" 
android:textColorHint="#4B4343" />
 <Button android:id="@+id/pass_forget" 
android:layout_width="wrap_content" 
android:layout_height="wrap_content"
 android:layout_below="@+id/password"
 android:layout_alignParentRight="true" 
android:layout_marginTop="10dp"
 android:backgroundTint="@android:color/transparent" 
android:text="forget Password?"
 android:textColor="@color/black"
 android:textSize="14dp" /> 

<Button
 android:id="@+id/login" 
android:layout_width="match_parent" 
android:layout_height="wrap_content" 
android:layout_below="@+id/pass_forget" 
android:layout_marginHorizontal="85dp" 
android:layout_marginTop="18dp" 
android:backgroundTint="#3F51B5"
 android:text="Login" 
android:textSize="28dp" />

 <Button
 android:id="@+id/create_acc" 
android:layout_width="wrap_content" 
android:layout_height="wrap_content" 
android:layout_below="@+id/login"
 android:layout_centerInParent="true" 
android:layout_marginTop="30dp" 
android:backgroundTint="@android:color/transparent"
 android:onClick="create_ac"
 android:text="Create new account" 
android:textColor="@color/black" 
android:textSize="16dp" 
android:textStyle="bold" />

 <TextView 
android:id="@+id/continue_with" 
android:layout_width="wrap_content" 
android:layout_height="wrap_content"
 android:layout_below="@+id/create_acc"
 android:layout_centerHorizontal="true"
 android:layout_marginTop="65dp"
 android:text="Or login with"
 android:textColor="#3F51B5"
 android:textStyle="bold" />

 <LinearLayout
 android:layout_width="match_parent"
 android:layout_height="wrap_content" 
android:layout_below="@+id/continue_with"
 android:layout_marginTop="10dp" 
android:gravity="center"> 

<ImageButton 
android:id="@+id/facebookButton"
 android:layout_width="40dp" 
android:layout_height="40dp" 
android:layout_below="@+id/continue_with" 
android:layout_margin="10dp"
 android:layout_marginLeft="85dp"
 android:background="@null"
 android:scaleType="centerInside" 
android:src="@drawable/fb" />

 <ImageButton 
android:id="@+id/google" 
android:layout_width="40dp" 
android:layout_height="40dp" 
android:layout_below="@+id/continue_with" 
android:layout_margin="10dp"
 android:layout_toRightOf="@+id/facebookButton"
 android:background="@null" 
android:scaleType="centerInside" 
android:src="@drawable/google" />

 <ImageButton 
android:id="@+id/twitter" 
android:layout_width="40dp" 
android:layout_height="40dp" 
android:layout_below="@+id/continue_with" 
android:layout_margin="10dp" 
android:layout_toRightOf="@+id/google" 
android:background="@null" 
android:scaleType="centerInside" 
android:src="@drawable/twitter" /> 
</LinearLayout>
</RelativeLayout>

login.java:
package com.example.haris_assignment2;
import android.content.Intent;
import android.os.Bundle;
import android.view.View;
import androidx.activity.EdgeToEdge;
import androidx.appcompat.app.AppCompatActivity;
import androidx.core.graphics.Insets;
import androidx.core.view.ViewCompat;
import androidx.core.view.WindowInsetsCompat;

public class MainActivity extends AppCompatActivity { 
public void create_ac(View view)
{ 
Intent intent = new Intent(this, signup_page.class); startActivity(intent); 
}
 @Override 
protected void onCreate(Bundle savedInstanceState) 
{
 super.onCreate(savedInstanceState); 
EdgeToEdge.enable(this); 
setContentView(R.layout.activity_main); 
ViewCompat.setOnApplyWindowInsetsListener(findViewById(R.id.main), (v, insets) 
-> {
 Insets systemBars = insets.getInsets(WindowInsetsCompat.Type.systemBars()); v.setPadding(systemBars.left, systemBars.top, systemBars.right, systemBars.bottom); return insets; });
 }
}



