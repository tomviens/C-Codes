# C-Codes
using UnityEngine;
using System.Collections;

public class Triggers : MonoBehaviour
{

    public Camera cam1;
    public Camera cam2;

    void OnTriggerEnter(Collider other)
    {

        if (other.gameObject.CompareTag("Player"))

        {
            cam2.enabled = false;
            cam1.enabled = true;
        }
    }
}
