using System.Collections;
using System.Collections.Generic;
using UnityEngine;

public class OnClick : MonoBehaviour
{
    public GameObject Origin;
    public GameObject Player;
    
    public void OnMouseDown()
    {
        Debug.Log("Teleporting player!");
        Player.transform.position = Origin.transform.position;
    }
}

