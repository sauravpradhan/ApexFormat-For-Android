# ApexFormat-For-Android
Procedure on how to convert a normal application source code to APEX format for android framework

1) Generate apex skeleton using : 
https://android.googlesource.com/platform/system/apex/+/refs/heads/master/tools/create_apex_skeleton.sh

2) Convert if project has .mk file to build to .bp file build 

    . build/envsetup.sh

    lunch

    m androidmk

    androidmk [flags] <inputFile>

3)  Add this to BP file "apex_available: ["myapexapp"]"

4) To Do  (Major ToDo when android 13 source is available)
