# MotionDetectionTrial
Python script to detect motion in a live video-feed.

This Pthon script uses a delta-threshold comparision to detect changes in the current frame, with the comparing frame logged at the
start of the script.

It then stores the data in an array (Start Time:, End Time:) to record each single instance of motion detected during the video feed, this
array is then converted into a Pandas dataframe which writes the readings to a "Time Map.csv" file.

The stored CSV file is then used to present the detected motions in a bar graph with:
  The left edge of the bar representing the start of an instance of detected motion and the left edge of the bar representing the end
  of an instance of detected motion.
  The height of the bar is the duration of the detected motion, although it can be set to any constant value as the X-axis shows the
  duration as well.

After this, the output graph is saved into the "Outputs" folder, which also stores the "Time Map.csv" file.
