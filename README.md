# EpreuveAtelierPandore

Blocage pendant plus de deux heures lors de la réalisation de l'exercice 2, suite à un problème avec la caméra AR. Celle-ci affiche un écran noir complet, bloquant l'utilisation des autres éléments de la scène. Après plusieurs recherches, l'erreur semble venir des avertissements suivants, présents dans la console :

• No active UnityEngine.XR.ARSubsystems.XRSessionSubsystem is available. Please ensure that a valid loader configuration exists in the XR project settings.
UnityEngine.XR.ARFoundation.ARSession:OnEnable () (at Library/PackageCache/com.unity.xr.arfoundation@4.2.3/Runtime/AR/ARSession.cs:341)

• No active UnityEngine.XR.ARSubsystems.XRCameraSubsystem is available. Please ensure that a valid loader configuration exists in the XR project settings.
UnityEngine.XR.ARFoundation.SubsystemLifecycleManager`3<UnityEngine.XR.ARSubsystems.XRCameraSubsystem, UnityEngine.XR.ARSubsystems.XRCameraSubsystemDescriptor, UnityEngine.XR.ARSubsystems.XRCameraSubsystem/Provider>:OnEnable () (at Library/PackageCache/com.unity.xr.arfoundation@4.2.3/Runtime/AR/SubsystemLifecycleManager.cs:68)

• No active UnityEngine.XR.ARSubsystems.XRRaycastSubsystem is available. Please ensure that a valid loader configuration exists in the XR project settings.
UnityEngine.XR.ARFoundation.ARTrackableManager`5<UnityEngine.XR.ARSubsystems.XRRaycastSubsystem, UnityEngine.XR.ARSubsystems.XRRaycastSubsystemDescriptor, UnityEngine.XR.ARSubsystems.XRRaycastSubsystem/Provider, UnityEngine.XR.ARSubsystems.XRRaycast, UnityEngine.XR.ARFoundation.ARRaycast>:OnEnable () (at Library/PackageCache/com.unity.xr.arfoundation@4.2.3/Runtime/AR/ARTrackableManager.cs:95)

• No active UnityEngine.XR.ARSubsystems.XRPlaneSubsystem is available. Please ensure that a valid loader configuration exists in the XR project settings.
UnityEngine.XR.ARFoundation.ARPlaneManager:OnEnable () (at Library/PackageCache/com.unity.xr.arfoundation@4.2.3/Runtime/AR/ARPlaneManager.cs:286)

• No active UnityEngine.XR.XRInputSubsystem is available. Please ensure that a valid loader configuration exists in the XR project settings.
UnityEngine.XR.ARFoundation.ARInputManager:OnEnable () (at Library/PackageCache/com.unity.xr.arfoundation@4.2.3/Runtime/AR/ARInputManager.cs:24)

Les tentatives suivantes de résolution du problème ont été mises en place, sans succès :

- Suppression et réinstallation des packages liées à l'AR Foundation ;
- Ajout du package Universal RP et modification des paramètres de rendering du projet ;
- Vérification des paramètres du projet, notamment concernant la section XR Plug-in Management, et plus particulièrement les paramètres Android (ARCore) ;
- Changement de version d'Android vers Windows ;
- Test remote du projet sur appareil Android branché à l'ordinateur par câble USB ;
- Mise à jour des packages ;
- Vérification de leur compatibilité avec la version d'Unity.

Impossibilité de mettre en place le système de réalité augmentée suite à ce problème.

----------------------------------------------------------------------------------------------------

Lien vers le Trello du projet : https://trello.com/invite/b/bIQXyjm5/c3447cd66787095499a024fb441e2406/epreuve-atelier-pandore
