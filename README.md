1.In the ./script, make a 2012_train.txt which include all names of training picutre. 
2.mkdir VOCdevkit/VOC2012
3.cd VOCdevkit/VOC2012
4.mkdir Annotations labels
5.The annotations include xxx.xml and the labels include xxxx.txt ( xxxx is the name of training picture)
6.cd $root
7.make
8.fllow the command 
      curl -O https://pjreddie.com/media/files/darknet19_448.conv.23
      ./darknet partial cfg/darknet19_448.cfg darknet19_448.weights darknet19_448.conv.23 23
9.Train the model
      ./darknet detector train cfg/voc.data cfg/yolo-voc.cfg darknet19_448.conv.23
10.For more informations, please go to https://pjreddie.com/darknet/yolo/
