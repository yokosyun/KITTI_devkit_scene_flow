## installation
download png++-0.2.9.tar.gz
http://download.savannah.nongnu.org/releases/pngpp/

untar

make && sudo make install

## compile
cd devkit /cpp
g++ -O3 -DNDEBUG -o evaluate_scene_flow evaluate_scene_flow.cpp -lpng

## evalate
please read evaluate_scene_flow.cpp the directory is annoying
./evaluate_scene_flow {result_path}

./evaluate_scene_flow KITTI/data_scene_flow/eval

*make sure you have result_data and traing_data with correct path


# result
 
D1_bg D1_bg_result D1_fg D1_fg_result D1_all D1_all_result density
0.037923 0.037923 0.049488 0.049488 0.039695 0.039695 1.000000

