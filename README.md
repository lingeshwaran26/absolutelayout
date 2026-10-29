# Develop an Android Application Using AbsoluteLayout Demonstrating Fixed Positioning


**Project Name:** AbsoluteLayout

## Aim

To develop an Android application using `AbsoluteLayout` to demonstrate fixed positioning of UI components.

## I. Filename: `activity_main.xml`

**Location:** `app/src/main/res/layout/activity_main.xml`

```xml
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:id="@+id/main"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">

    <AbsoluteLayout
        android:layout_width="408dp"
        android:layout_height="728dp"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.497"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.139">

        <TextView
            android:id="@+id/textView"
            android:layout_width="275dp"
            android:layout_height="54dp"
            android:layout_x="60dp"
            android:layout_y="30dp"
            android:text="Absolute Layout Demo"
            android:textAlignment="center"
            android:textSize="24sp"
            android:textStyle="bold" />

        <TextView
            android:id="@+id/textView2"
            android:layout_width="87dp"
            android:layout_height="40dp"
            android:layout_x="30dp"
            android:layout_y="100dp"
            android:text="Name"
            android:textAlignment="center"
            android:textSize="20sp" />

        <TextView
            android:id="@+id/textView3"
            android:layout_width="87dp"
            android:layout_height="40dp"
            android:layout_x="30dp"
            android:layout_y="170dp"
            android:text="Email"
            android:textAlignment="center"
            android:textSize="20sp" />

        <EditText
            android:id="@+id/editTextText"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_x="100dp"
            android:layout_y="90dp"
            android:ems="10"
            android:inputType="text"
            android:text="Enter Name" />

        <EditText
            android:id="@+id/editTextText1"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_x="100dp"
            android:layout_y="160dp"
            android:ems="10"
            android:inputType="text"
            android:text="Enter Email" />

        <Button
            android:id="@+id/button"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_x="50dp"
            android:layout_y="250dp"
            android:text="Submit" />

        <Button
            android:id="@+id/button2"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_x="190dp"
            android:layout_y="250dp"
            android:text="Reset" />

    </AbsoluteLayout>

</androidx.constraintlayout.widget.ConstraintLayout>
```

## Explanation

1. **ConstraintLayout:** Acts as the parent container and positions the `AbsoluteLayout` within the screen.
2. **AbsoluteLayout:** Positions child components using fixed X and Y coordinates.
3. **TextView:** Displays the heading "Absolute Layout Demo" and the labels Name and Email.
4. **EditText:** Allows users to enter their name and email.
5. **Submit Button:** Provides an interface for submitting the entered details.
6. **Reset Button:** Provides an interface for resetting the input fields.
7. **`android:layout_x` and `android:layout_y`:** Specify the horizontal and vertical positions of components within the `AbsoluteLayout`.

## Output

The application displays a form containing:

- A heading at the top.
- Name and Email labels.
- Input fields for Name and Email.
- Submit and Reset buttons positioned using fixed coordinates.

## Result

Thus, an Android application demonstrating fixed positioning using `AbsoluteLayout` was designed successfully.

## Note

`AbsoluteLayout` is deprecated in Android because fixed coordinates may cause UI elements to overlap or appear incorrectly on screens of different sizes. Modern Android applications should generally use `ConstraintLayout` or other responsive layouts instead.
