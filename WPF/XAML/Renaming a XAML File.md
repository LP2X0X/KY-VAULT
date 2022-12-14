- Renaming items in Visual Studio can break the code if we’re not careful. To maintain the appropriate links between the files when renaming the window, do the following:
	- Select < old name >.xaml in the Solution Explorer.
	- Press F2 on your keyboard. (Alternatively, you can right-click and select Rename.)
	- Change the filename to MainWindow.xaml. Note that Visual Studio renames the associated code-behind as well. However, Visual Studio does not correct references to the filename, nor does it change the name of the underlying class.
	- Double-click App.xaml in the Solution Explorer to open it in the editor.
	- The root tag in App.xaml is the Application tag, and it has an attribute StartupUri. StartupUri specifies the name of the primary window that is displayed when the application launches. It’s still pointing to the old name; change it to point to < new name >.xaml
	- Open the code-behind for < new name >.xaml in the editor; that’s < new name >.xaml.cs. Notice that the class is still named < old name >. Renaming the XAML file did not change the name of the class.
	- To avoid confusion, we’ll change the name of the class to match the name of the file.
	- Finally, in the markup for < new name >.xaml, we need to correct the reference to the class. We need to change this to the full name of our class, including the namespace, which is < project name >.< new name >.