# RootBranch_HPWREN_Results

This dataset contains six test videos selected from the article "Video Smoke Detection Method Based on Cell Root-Branch Structure" and the test results of the method proposed in the article on the HPWREN dataset.

There are three main folders:

**HPWREN_Dataset**: Contains the five time-lapse segments that make up Video4.
20210810-Lyonsfire-housefire-lp-n-mobo-c: Lyonsfire that occurred in LP on August 10, 2021.
20220214-PrescribedFire-pi-n-mobo-c: PrescribedFire that occurred in PI on February 14, 2022.
20220713-Lonestarfire-om-w-mobo-c: Lonestarfire that occurred in OM on July 13, 2022.
20230806-PassFire-ws-n-mobo-c: PassFire that occurred in WS on August 6, 2023.
20230809-BunnieFire-cp-w-mobo-c: BunnieFire that occurred in CP on August 9, 2023.

**TestResults**: Contains the test results of the method proposed in the article on the HPWREN dataset (Video4).
There are 5 folders, each corresponding to the names of the 5 video files in the HPWREN_Dataset.
Each folder contains 7 subfolders, corresponding to the 7 stages of processing results in our method.
1_OriginalImage: Frame-by-frame output of the original video (color images).
2_MotionFilter: Results of motion foreground detection on the original video (binary images, white represents motion areas).
3_ColorFilter: Results of color threshold filtering on the original video (binary images, white represents smoke color areas).
4_FilterResults: Results of bitwise AND operation on the foreground detection mask and smoke color mask (binary images, white represents areas preliminarily screened as possible smoke).
5_GridsStructure: Constructed Cell Root-Branch Structure (color images).
6_GridsCounter: Grid count results combined with spatio-temporal context information (color images).
7_FinalResults: Final smoke detection results (color images, smoke is marked with green anchor boxes).

**TestVideo**: Contains Videos 1, 2, 3, 5, and 6 mentioned in the article. The video format is .mp4.
