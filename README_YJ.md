# Line by line

roslaunch elevation_mapping_demos cassie_demo.launch

roslaunch elevation_mapping_demos remap_tfs.launch

rosservice call /elevation_mapping/save_map "file_path: '/home/youngji/workspace/maps/cassie2/elevation_map_full1.bag' 
topic_name: 'elevation_map'"

rosservice call /elevation_mapping/clear_map

# Automatic submap savings


roslaunch elevation_mapping_demos cassie_demo.launch

roslaunch elevation_mapping_demos remap_tfs.launch

rosservice call /elevation_mapping/save_and_clear_map "file_path: '/home/youngji/workspace/maps/cassie2/elevation/'"
