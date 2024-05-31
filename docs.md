## Output after extraction 
- **bboxes_p**: This variable contains the bounding boxes of detected players, referees, and balls in the format (x1, y1, x2, y2), where (x1, y1) is the top-left corner and (x2, y2) is the bottom-right corner of the bounding box.

- **bboxes_p_c**: This variable contains the bounding boxes of detected players, referees, and balls in the format (x, y, w, h), where (x, y) is the top-left corner and (w, h) is the width and height of the bounding box.

- **labels_p**: This variable contains a list of labels for the detected players, referees, and balls. The labels are numerical.

- **confs_p**: This variable contains a list of confidence levels for the detected players, referees, and balls.

- **bboxes_k**: This variable contains the bounding boxes of detected field keypoints in the format (x1, y1, x2, y2), where (x1, y1) is the top-left corner and (x2, y2) is the bottom-right corner of the bounding box.

- **bboxes_k_c**: This variable contains the bounding boxes of detected field keypoints in the format (x, y, w, h), where (x, y) is the top-left corner and (w, h) is the width and height of the bounding box.

- **labels_k**: This variable contains a list of numerical labels for the detected field keypoints.

- **detected_labels**: This variable contains a list of alphabetical labels for the detected field keypoints. These labels are obtained by converting the numerical labels in labels_k to alphabetical labels using a dictionary classes_names_dic.

- **detected_labels_src_pts**: This variable contains the coordinates of the detected field keypoints on the current frame. These coordinates are extracted from the top-left corner of the bounding boxes in bboxes_k_c.

- **detected_labels_dst_pts**: This variable contains the coordinates of the detected field keypoints on the tactical map. These coordinates are obtained by mapping the alphabetical labels in detected_labels to their corresponding positions on the tactical map using a dictionary keypoints_map_pos.