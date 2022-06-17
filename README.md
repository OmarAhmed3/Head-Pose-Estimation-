# Head-Pose-Estimation-
Head Pose Estimation project 

# Description 
## detecting a person if person look left or right or upper and down using mediapipe library by three Angles (pitch , yaw , roll) two angle vertical Nose and other angle change from position to postion.

# Steps 

## 1.  import mediapipe and cv2 
## 2.  looping to collect paths  of dataset in list using os.listdir and path of directory of dataset and append this paths in list(paths)
## 3.  looping to paths list and using imread.csv , holistic.process ,  mp_drawing.draw_landmarks to get coordinates of points (x , y , z)
## 4.  we looping for this points and get (x,y) points and we add three Angles (pitch, yaw , roll)
## 5.  we prepare csv.file to read dataset in this csv file 
## 6.  we read matfile and we insert this reading in csvfile (Landmarks_data.csv)
## 7.  we read a csvfile of data using pandas and drop labels of dataset(three Angle) and we get shape of dataset (1137, 939)
## 8.  we divide dataset by train_test_split to test_data , validation_data and test_data
## 9.  we train models using pipelines 
## 10. we Normalize data using StandardScaler
## 11. we use PCA and RandomForestRegressor model to get predictions 
## 12. we training pipeline and get error of points 
## 13. we load this models using pickle.load() to ready to using webcam 
## 14. we using cv2 and landmarks to predict models in face_row from data
## 15. we make alot of equations to draw three coordinates (Three Angle)
## 16. X-Axis pointing to right. drawn in red
## 17. Y-Axis | drawn in green
## 18. Z-Axis (out of the screen) drawn in blue
## 19. we using webcam live to detect position of person



