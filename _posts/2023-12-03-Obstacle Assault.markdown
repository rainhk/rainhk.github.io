---
layout: post
title:  "UE5 3rd Project"
date:   2023-12-03 00:00:00 +0530
categories: Project
---
UE5 3rd project

<br>

# Obstacle Assault
This was a 3rd UE project to understand blueprint and programming with C++ .\
\
![stack](/assets/video/ObstacleAssault - Unreal Editor 2024-01-15 21-03-05.mp4)
Please wait a few seconds to load video!
<br>

## On this project, I've learned...
1. How to modify code to add desired features\
    \* Added moving and rotating platform feature <br>
    \* Learned speed and object movements <br>
    \* Learned how to see Logs
2. How to implement character collision\
    \* Modify MoveUpdatedComponent to move character front and back by 1 pixel
    
<br>
Below is code for moving platforms
``` cpp
void AMovingPlatform::MovePlatform(float DeltaTime)
{
        // Reverse direction of motion if gone too far
    if (ShouldPlatformReturn())
    {    
        FVector MoveDirection = PlatformVelocity.GetSafeNormal();
        StartLocation = StartLocation + MoveDirection * MoveDistance;
        SetActorLocation(StartLocation);
        PlatformVelocity = -PlatformVelocity;
    } 
    else 
    {
        // Move platform forwards
        // Get current location
    FVector CurrentLocation = GetActorLocation();
        // Add vector to that location
    CurrentLocation += PlatformVelocity*DeltaTime;
        // Set the location
    SetActorLocation(CurrentLocation);
    // Send platform back if gone too far
        // check how far we've moved
    }
}

void AMovingPlatform::RotatePlatform(float DeltaTime)
{
    AddActorLocalRotation(RotationVelocity * DeltaTime);
}
```


\* add video of a map designed
