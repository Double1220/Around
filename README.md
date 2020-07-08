# Around
In this project, I use Go to build a scalable web service that has three APIs: post, search, and cluster. 
The following figure shows the overall architecture of this program:

 <img src="https://github.com/Double1220/Around/blob/master/Images/Architecture.JPG" width="650" height="500">

1. The post API allows users to submit a post. and the post consists a description message, geolocation info and media file. 
After posting, the media file will store to GCS and other info will be stored at ES
2. The search API allows users to search nearby posts based on their current location. And this function is realized by connecting our program to Elasticsearch. 
3. The cluster API allows users to filter face -related posts by using Google cloud vision API. 

This application provides functions shown as the following:
1. Login to the system
  ![image](https://github.com/Double1220/Around/blob/master/Images/Login.JPG) 
2. when user login to the system, the user can choose to upload posts from local computer.
  ![image](https://github.com/Double1220/Around/blob/master/Images/Post.JPG) 
3. After choosing which file to be uploaded, the user can add one description message to this post, and then upload it.
  ![image](https://github.com/Double1220/Around/blob/master/Images/post%20msg.JPG) 
4. Then user can check all uploaded images.
  ![image](https://github.com/Double1220/Around/blob/master/Images/posted%20img.JPG) 
5. Also, provided a botton to present face-related posts direclty
 ![image](https://github.com/Double1220/Around/blob/master/Images/Face%20only.JPG) 
6. User can also check nearby posts.
 ![image](https://github.com/Double1220/Around/blob/master/Images/Map.JPG) 

 Please feel free to download it and develope it! If you have any questions, please contact me at lllaioffer@gmail.com.
