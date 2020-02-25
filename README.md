# Navigation graph
The Navigation Graph is an XML resource type. It includes a visual editor that allows drag & drop representation of fragment.
- In Project hierarchy <br />
  ![Captura de Pantalla 2020-02-25 a la(s) 4 52 13 p  m](https://user-images.githubusercontent.com/10893692/75291492-53ec8b00-57f0-11ea-91f7-9c9df9007426.png)
- Visual editor <br />
  ![Captura de Pantalla 2020-02-25 a la(s) 4 52 55 p  m](https://user-images.githubusercontent.com/10893692/75291801-f0169200-57f0-11ea-8aab-852274504adb.png)

# Destination
The screens are called destinations or where you want to move.
![Captura de Pantalla 2020-02-25 a la(s) 4 52 55 p  m](https://user-images.githubusercontent.com/10893692/75293314-ef332f80-57f3-11ea-9c7e-fc1a171cf945.png)

# Action
The arrows represent the `action` that defines the navigation route. When clicking on the arrow you’ll get several options including `animation transition`, `defining destination`, `backstack manipulation` and data passing between destinations.
![Captura de Pantalla 2020-02-25 a la(s) 5 27 58 p  m](https://user-images.githubusercontent.com/10893692/75293544-636dd300-57f4-11ea-9aad-566a04a40557.png)

# Navigation Host Fragment
Is a widget or screen that provides hosting to your navigation graph. This means that all of the defined navigation in the navigation graph is run on it.<br/>
You need to define nav. host fragment in an Activity in the following way:
```
<fragment
    android:id="@+id/nav_host_fragment"
    ...........
    android:name="androidx.navigation.fragment.NavHostFragment"
    app:defaultNavHost="true"
    app:navGraph="@navigation/navigation_graph" />
```
`app:navGraph="@navigation/navigation_graph` ==> (Is the same XML resource)
