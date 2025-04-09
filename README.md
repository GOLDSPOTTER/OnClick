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
        GameObject Camera = GameObject.Find("FallbackObjects");
        if (Camera != null)
        {
            Player.transform.position = Origin.transform.position;
            Camera.transform.localPosition = new Vector3(0, 1.75f ,0);
        }
    }
}
