# Ex.No: 2  Welcome Script in Unity
### DATE:  25/07/26                                                                          
### REGISTER NUMBER : 212224230314
### AIM: 
 To learn the basic scripting in Unity and print welcome message in Console window. 
### Procedure:
1. Start the program
2. Open the Unity hub and Create a new 3D project
3. In Assets window, create the new folder and name it as Scripts
4. Create a new script with file name as FirstScript
5. Open the Script and print message "Welcome to Unity" inside the start function
6. Save the script
7. Create a new 3D game object in Hierarchy window and name it as 3DObject.
8. Add the component Firstscript in inspector window of 3Dobject.
9. Run the program
10. Stop the program.
### Program 
```
{
    public Transform o1;
    public Transform o2;
    public Transform o3;
    void Start()
    {
        print("Welcome");
    }

    // Update is called once per frame
    void Update()
    {
        //  print("Welcome to unity");

        o1.Translate(2f, 0, 0);
        o2.Rotate(0, 10f, 0);
        o3.localScale+=new Vector3(0.2f, 0.2f, 0.2f);
    
    }

}
```
### Output:

<img width="1917" height="1078" alt="Screenshot 2026-07-24 082757" src="https://github.com/user-attachments/assets/890b5763-b36a-44ed-b372-c60b216cdd77" />


### Result:
Thus the welcome script was printed on Console Window  sucessfully.

