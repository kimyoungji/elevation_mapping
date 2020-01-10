roslaunch elevation_mapping_demos simple_demo.launch

rosservice call /elevation_mapping/save_map "file_path: '/home/youngji/elevation_map.bag' 
topic_name: 'elevation_map'"

