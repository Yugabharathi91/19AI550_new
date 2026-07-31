# Ex.No: 6  Implementation of Jumping  behaviour- Unity
### DATE: 31/072026                                                                           
### REGISTER NUMBER : 212224230314
### AIM: 
To write a program to simulate the process of jumping in Unity.
### Algorithm:
```
1. Create a new 3D Unity project
2. Add a Plane
3. Right-click Hierarchy → 3D Object → Plane → Rename to Ground
4. Add a Cube (Player)
5. Right-click Hierarchy → 3D Object → Cube → Rename to Player
6. Set Position: (0, 0.5, 0)
7. Add a Rigidbody to the Player
8. With the Player selected: Inspector → Add Component → Rigidbody
9. Set Constraints > Freeze Rotation X, Z (optional for stability)
10.Create the Jump Script and Apply the Script Player
11.Run the game
Press Play
Press Spacebar to jump
Your cube should only jump when touching the ground
```
###
**Program **
```
using UnityEngine;

public class PlayerJump : MonoBehaviour
{
    private Rigidbody rb;
    public float jumpForce = 5f;
    
    void Start()
    {
        rb = GetComponent<Rigidbody>();
    }

    void Update()
    {
        if (Input.GetKeyDown(KeyCode.Space) )
        {
            rb.AddForce(Vector3.up * jumpForce, ForceMode.Impulse);
            
        }
    }

   
}
```
### Output:




<img width="1916" height="1015" alt="628245696-6b48c864-0919-40bd-a404-ea3392e5b6b1" src="https://github.com/user-attachments/assets/226d8119-2d27-4211-b1bf-2b9248d0896e" />
<img width="1917" height="1020" alt="628245706-8d4fe3dd-2cf1-4452-837e-e7ed203763a8" src="https://github.com/user-attachments/assets/26470fb6-604a-472e-a465-a306b6dd9ecd" />





### Result:
Thus the simple jumping behavior was implemented successfully.
