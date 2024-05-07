# Participant Data

Participant data is located in the Path_Data directory. Each xdf file contains the data streams for a single participant. Data was collected using the LabRecorder application for the LabStreamingLayer (LSL) protocol. 

The data streams are as follows:
- `LuminanceStream`: The luminance values of the screen (measured on compute shader from xyz color space)
- `GazeStream`: The gaze data of the participant
- `NavigationStream`: Data from navigation tasks
- `CreationStream`: Data from creation tasks
- `SurveyStream`: Data from creation and navigation surveys
- `PoseStream`: The world-space pose of the participant's head and hands
- `TrackedPoseStream`: The tracking pose data of the participant's head and hands
- `ExperimentStream`: Generic events from the experiment, including handedness and scene entry/exit logs. Due to nuances in how SteamVR renders OpenXR appliations, the "SceneStart" events can fire twice during asynchronous scene loading. 


## Data Notes

- Pilot participants are #100-107
    - 100: RTX 2080. Run in editor, different locomotion parameters, no gaze calibration.
    - 101: RTX 2080. Different locomotion parameters, no gaze calibration.
    - 102: RTX 2080. Different locomotion parameters, no gaze calibration.
    - 103: RTX 2080. Different locomotion parameters, no gaze calibration.
    - 104: RTX 2080. Different locomotion parameters, no gaze calibration.
    - 105: RTX 2080. Different locomotion parameters, no gaze calibration.
    - 106: RTX 3080. No gaze calibration.
    - 107: RTX 3080. No gaze calibration.
- Additional exclusions: 
    - 113: Eye tracking/SteamVR crash during second navigation task. 
    - 115: Discontinued due to FMS score of 10. 
    - 130: Pulled the HMD cord out of the computer (???) during the second planning task. Could not recover experiment. 
    - 138: Discontinued due to FMS score of 10. 