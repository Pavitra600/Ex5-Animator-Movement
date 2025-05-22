# Ex5-Animator-Movement

## Aim:
To develop a animator movement for a player using unity.

## Algorithm:
## Step 1:
Import necessary models.

## Step 2:
Right-click -> Create -> Animator Controller.

## Step 3:
Open Animator window, define states (Idle, Run, Jump, etc.).

## Step 4:
Use keyframes or Unity's Animation tools to animate transitions between states.

## Step 5:
Drag Animator Controller to the GameObject in the Inspector.

## Program:
## Developed by: PAVITRA. J
## Reg no: 212224110043
## Animator
```
using UnityEngine;

public class Movement : MonoBehaviour
{
    public Animator animator;
    public float InputX;
    public float InputY;

    void Start()
    {
        animator  = this.gameObject.GetComponent<Animator>();
        
    }
    void Update()
    {
        InputY = Input.GetAxis("Vertical");
        InputX = Input.GetAxis("Horizontal");
        animator.SetFloat("InputY",InputY);
        animator.SetFloat("InputX",InputX);
    }
}

```
## Output:
![Screenshot (31)](https://github.com/user-attachments/assets/b72eb255-cc88-43a6-b1a4-7e66bbf51091)
![Screenshot (33)](https://github.com/user-attachments/assets/3dd627f7-af21-46ed-9652-92c116081067)
![Screenshot (32)](https://github.com/user-attachments/assets/16f8ed0b-b9a3-48f8-a644-d5f7f64f46ed)


## Result:

An animator movement for a player using unity is developed successfully.
