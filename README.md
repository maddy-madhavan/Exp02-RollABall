# Exp02-RollABall
Developed by: MADHAVAN K

Register number: 212224220054
# Aim:
To develop a 3D application for Roll A Ball in unity.

# Procedure:
# Step1:
Create a new project.

# Step 2:
Click Heirarchy -> 3D object -> Select the plane -> 3DObject -> Sphere.

# Step 3:
Define the physics properties of the surface (Rigidbody).

# Step 4:
Assets -> Create -> # Script

# Step 5:
Create a folder name Coding and create a C# file to add the coding in it.

# Step 6:
To add our C# Script file to our selected object, click on the C# Script file and drag it to our selected objects in the Hierarchy window nad run the application.

# Step 7:
Stop.

# Program:
```
using System.Collections;
using System.Collections.Generic;
using UnityEngine;

public class Code : MonoBehaviour
{
    public float Xforce =5.0f;
       public float Zforce =5.0f;
       public float Yforce =100.0f; 
    // Start is called before the first frame update
    void Start()
    {
       
    }

    // Update is called once per frame
    void Update()
    {
        float X=0.0f,Y=0.0f,Z=0.0f;
        if(Input.GetKey(KeyCode.A))
        {
            X=X-Xforce;

        }
        if(Input.GetKey(KeyCode.D))
        {
            X=X+Xforce;
        }
        if(Input.GetKey(KeyCode.A))
        {
            Z=Z-Zforce;
        }
        if(Input.GetKey(KeyCode.D))
        {
            Z=Z+Zforce;
        }
        if(Input.GetKeyDown(KeyCode.Space))
        {
            Y=Yforce;
        }
        GetComponent<Rigidbody>().AddForce(X,Y,Z);
    }
}
```

# Output:

![alt text](<Screenshot 2025-04-23 215620.png>)
# Result:
Thus, a 3D application for RollABall objects in unity is developed successfully.