实验二Android布局实验——线性布局
01：线性布局：

<?xml version="1.0" encoding="utf-8"?>

<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:tools="http://schemas.android.com/tools"
    android:orientation="vertical"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:background="#000000">
    <LinearLayout
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:orientation="horizontal">
        <Button
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:background="@drawable/shape"
            android:layout_marginTop="3dip"
            android:layout_marginLeft="3dip"
            android:textColor="#ffffff"

            tools:text="one,one" />
        <Button
            android:layout_width="120dip"
            android:layout_height="wrap_content"
            android:background="@drawable/shape"
            android:layout_marginTop="3dip"
            android:layout_marginLeft="3dip"
            android:textColor="#ffffff"
            tools:text="one,two" />
        <Button
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:background="@drawable/shape"
            android:textColor="#ffffff"
            android:layout_marginTop="3dip"
            android:layout_marginLeft="3dip"
            tools:text="one,three" />
        <Button
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:background="@drawable/shape"
            android:textColor="#ffffff"
            android:layout_marginTop="3dip"
            android:layout_marginLeft="3dip"
            tools:text="one,four" />
    </LinearLayout>
    <LinearLayout
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:orientation="horizontal">
        <Button
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:background="@drawable/shape"
            android:layout_marginTop="3dip"
            android:layout_marginLeft="3dip"
            android:textColor="#ffffff"
            tools:text="two,one" />
        <Button
            android:layout_width="120dip"
            android:layout_height="wrap_content"
            android:background="@drawable/shape"
            android:layout_marginTop="3dip"
            android:layout_marginLeft="3dip"
            android:textColor="#ffffff"
            tools:text="two,two" />
        <Button
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:background="@drawable/shape"
            android:textColor="#ffffff"
            android:layout_marginTop="3dip"
            android:layout_marginLeft="3dip"
            tools:text="two,three" />
        <Button
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:background="@drawable/shape"
            android:textColor="#ffffff"
            android:layout_marginTop="3dip"
            android:layout_marginLeft="3dip"
            tools:text="two,four" />
    </LinearLayout>
    <LinearLayout
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:orientation="horizontal">
        <Button
            android:layout_width="100dip"
            android:layout_height="wrap_content"
            android:background="@drawable/shape"
            android:layout_marginTop="4dip"
            android:layout_marginLeft="3dip"
            android:textColor="#ffffff"
            tools:text="three,one" />
        <Button
            android:layout_width="90dip"
            android:layout_height="wrap_content"
            android:background="@drawable/shape"
            android:layout_marginTop="4dip"
            android:layout_marginLeft="3dip"
            android:textColor="#ffffff"
            tools:text="three,two" />
        <Button
            android:layout_width="100dip"
            android:layout_height="wrap_content"
            android:background="@drawable/shape"
            android:textColor="#ffffff"
            android:layout_marginTop="4dip"
            android:layout_marginLeft="3dip"
            tools:text="three,three" />
        <Button
            android:layout_width="95dip"
            android:layout_height="wrap_content"
            android:background="@drawable/shape"
            android:textColor="#ffffff"
            android:layout_marginTop="4dip"
            android:layout_marginLeft="3dip"
            tools:text="three,four" />
    </LinearLayout>
    <LinearLayout
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:orientation="horizontal">
        <Button
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:background="@drawable/shape"
            android:layout_marginTop="3dip"
            android:layout_marginLeft="3dip"
            android:textColor="#ffffff"
            tools:text="four,one" />
        <Button
            android:layout_width="120dip"
            android:layout_height="wrap_content"
            android:background="@drawable/shape"
            android:layout_marginTop="3dip"
            android:layout_marginLeft="3dip"
            android:textColor="#ffffff"
            tools:text="four,two" />
        <Button
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:background="@drawable/shape"
            android:textColor="#ffffff"
            android:layout_marginTop="3dip"
            android:layout_marginLeft="3dip"
            tools:text="four,three" />
        <Button
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:background="@drawable/shape"
            android:textColor="#ffffff"
            android:layout_marginTop="3dip"
            android:layout_marginLeft="3dip"
            tools:text="four,four" />
    </LinearLayout>
</LinearLayout>



02：约束布局
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:id="@+id/linearLayout"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:layout_weight="match_parent"
    android:orientation="vertical">

    <androidx.constraintlayout.widget.Guideline
        android:id="@+id/guideline5"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:orientation="horizontal"
        app:layout_constraintGuide_end="502dp" />

    <Button

        android:id="@+id/button"
        android:layout_width="395dp"
        android:layout_height="52dp"
        android:background="#D6C092"
        android:text="                                                                                                        0.0"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.163"
        tools:layout_editor_absoluteX="8dp" />

    <Button
        android:id="@+id/button2"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginTop="200dp"
        android:layout_marginBottom="52dp"
        android:text="7"
        app:layout_constraintBottom_toTopOf="@+id/button3"
        app:layout_constraintTop_toTopOf="parent"
        tools:layout_editor_absoluteX="8dp" />

    <Button
        android:id="@+id/button3"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginTop="60dp"
        android:text="4"
        app:layout_constraintTop_toBottomOf="@+id/button2"
        tools:layout_editor_absoluteX="8dp" />

    <Button
        android:id="@+id/button4"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginTop="60dp"
        android:text="1"
        app:layout_constraintTop_toBottomOf="@+id/button3"
        tools:layout_editor_absoluteX="8dp" />

    <Button
        android:id="@+id/button5"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginTop="60dp"
        android:text="."
        app:layout_constraintTop_toBottomOf="@+id/button4"
        tools:layout_editor_absoluteX="8dp" />

    <Button
        android:id="@+id/button6"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginTop="200dp"
        android:text="8"
        app:layout_constraintTop_toTopOf="parent"
        tools:layout_editor_absoluteX="107dp" />

    <Button
        android:id="@+id/button7"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginTop="60dp"
        android:text="5"
        app:layout_constraintTop_toBottomOf="@+id/button6"
        tools:layout_editor_absoluteX="107dp" />

    <Button
        android:id="@+id/button8"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginTop="60dp"
        android:text="2"
        app:layout_constraintTop_toBottomOf="@+id/button7"
        tools:layout_editor_absoluteX="107dp" />

    <Button
        android:id="@+id/button9"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginStart="11dp"
        android:layout_marginLeft="11dp"
        android:layout_marginTop="60dp"
        android:text="0"
        app:layout_constraintStart_toEndOf="@+id/button5"
        app:layout_constraintTop_toBottomOf="@+id/button8" />

    <Button
        android:id="@+id/button10"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginTop="200dp"
        android:text="9"
        app:layout_constraintBottom_toTopOf="@+id/button11"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.0"
        tools:layout_editor_absoluteX="215dp" />

    <Button
        android:id="@+id/button11"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginTop="60dp"
        android:text="6"
        app:layout_constraintTop_toBottomOf="@+id/button10"
        tools:layout_editor_absoluteX="215dp" />

    <Button
        android:id="@+id/button12"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginTop="60dp"
        android:text="3"
        app:layout_constraintTop_toBottomOf="@+id/button11"
        tools:layout_editor_absoluteX="215dp" />

    <Button
        android:id="@+id/button13"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginTop="60dp"
        android:text="="
        app:layout_constraintTop_toBottomOf="@+id/button12"
        tools:layout_editor_absoluteX="215dp" />

    <Button
        android:id="@+id/button14"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginStart="11dp"
        android:layout_marginLeft="11dp"
        android:layout_marginTop="200dp"
        android:text="÷"
        app:layout_constraintStart_toEndOf="@+id/button10"
        app:layout_constraintTop_toTopOf="parent" />

    <Button
        android:id="@+id/button15"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginStart="11dp"
        android:layout_marginLeft="11dp"
        android:layout_marginTop="60dp"
        android:text="×"
        app:layout_constraintStart_toEndOf="@+id/button11"
        app:layout_constraintTop_toBottomOf="@+id/button14" />

    <Button
        android:id="@+id/button16"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginTop="60dp"
        android:text="+"
        app:layout_constraintTop_toBottomOf="@+id/button15"
        tools:layout_editor_absoluteX="313dp" />

    <Button
        android:id="@+id/button17"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginStart="11dp"
        android:layout_marginLeft="11dp"
        android:layout_marginTop="60dp"
        android:text="-"
        app:layout_constraintStart_toEndOf="@+id/button13"
        app:layout_constraintTop_toBottomOf="@+id/button16" />

    <TextView
        android:textSize="28dp"
        android:id="@+id/textView"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginStart="16dp"
        android:layout_marginLeft="16dp"
        android:text="Input"
        app:layout_constraintStart_toStartOf="parent"
        tools:layout_editor_absoluteY="33dp" />

</androidx.constraintlayout.widget.ConstraintLayout>



03：表格布局
<?xml version="1.0" encoding="utf-8"?>
<TableLayout xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:stretchColumns="1"
    android:background="#000000">

    <TableRow>
        <TextView
            android:layout_column="1"
            android:text="Open..."
            android:padding="3dip"
            android:textColor="#ffffff"/>
        <TextView
            android:text="Ctrl-O"
            android:gravity="right"
            android:padding="3dip"
            android:textColor="#ffffff"/>

    </TableRow>

    <TableRow>
        <TextView
            android:layout_column="1"
            android:text="Save..."
            android:padding="3dip"
            android:textColor="#ffffff"/>
        <TextView
            android:text="Ctrl-S"
            android:gravity="right"
            android:padding="3dip"
            android:textColor="#ffffff"/>
    </TableRow>

    <TableRow>
        <TextView
            android:layout_column="1"
            android:text="Save As..."
            android:padding="3dip"
            android:textColor="#ffffff"/>
        <TextView
            android:text="Ctrl-Shift-S"
            android:gravity="right"
            android:padding="3dip"
            android:textColor="#ffffff"/>
    </TableRow>

    <View
        android:layout_height="2dip"
        android:background="#ffffff"/>
    <TableRow>
        <TextView
            android:text="X"
            android:textColor="#ffffff"
            android:padding="3dip"/>
        <TextView
            android:text="Import..."
            android:textColor="#ffffff"
            android:padding="3dip"/>
    </TableRow>
    <TableRow>
        <TextView
            android:text="X"
            android:textColor="#ffffff"
            android:padding="3dip"/>
        <TextView
            android:text="Emport..."
            android:textColor="#ffffff"
            android:padding="3dip"/>
        <TextView
            android:text="Ctrl-E"
            android:gravity="right"
            android:textColor="#ffffff"
            android:padding="3dip"/>
    </TableRow>
    <View
        android:layout_height="2dip"

        android:background="#ffffff"/>
    <TableRow>
        <TextView
            android:layout_column="1"
            android:textColor="#ffffff"
            android:text="Quit"
            android:padding="3dip"/>
    </TableRow>
</TableLayout>
