$\quad$Model–view–viewmodel (MVVM) is an [[Architectural Pattern]] in computer software that facilitates the separation of the development of the Graphical User Interface (GUI; the view) — be it via a markup language or GUI code — from the development of the business logic or back-end logic (the model) such that the view is not dependent upon any specific model platform. 
![[Pasted image 20221209133046.png|center]]
- The benefits of using the MVVM pattern are as follows:
	    - If an existing model implementation encapsulates existing business logic, it can be difficult or risky to change it. In this scenario, the view model acts as an adapter for the model classes and prevents you from making major changes to the model code.
	    - Developers can create unit tests for the view model and the model, without using the view. The unit tests for the view model can exercise exactly the same functionality as used by the view.
	    - The app UI can be redesigned without touching the view model and model code, provided that the view is implemented entirely in XAML or C#. Therefore, a new version of the view should work with the existing view model.
	    - Designers and developers can work independently and concurrently on their components during development. Designers can focus on the view, while developers can work on the view model and model components.
