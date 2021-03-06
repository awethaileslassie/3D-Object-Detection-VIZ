3D Bounding box visualization with point clouds in Python
=========================================================

Requirment
==========
By itself Mayavi is not a difficult package to install but its dependencies
are unfortunately rather heavy. However, many of these dependencies are now
available as wheels on PyPI.  The two critical dependencies are,
```
  1. VTK_
  2. A GUI toolkit, either PyQt4_, PySide_, PySide2_, PyQt5_ or wxPython_.
```

Installation
============
```
  conda create -n mayavi python==3.6
  conda activate mayavi
  git clone https://github.com/awethaileslassie/3D-Object-Detection-VIZ.git
  cd 3D-Object-Detection-VIZ/mayavi
  pip install -r requirements.txt
  pip install PyQt5  # replace this with any supported toolkit
  python setup.py install  # or develop

```

Demo
====
```
conda activate mayavi

cd  3D-Object-Detection-VIZ/mayavi

mayavi2 -x plot_3D_bbox.py
```

How to Use
==========
First change the input pcl directory and labels directory inside the "plot_3D_bbox.py" to your own file
```
pc = np.load('data/lidar/2011_09_26_0036_0030.npy')
bbox = np.load('data/label/2011_09_26_0036_0030.npy')
```

```
conda activate mayavi

cd  3D-Object-Detection-VIZ/mayavi

mayavi2 -x plot_3D_bbox.py
```

You will see some visulization which looks like this
![Image description](kitti.png)


# 3D-Object-Detection-VIZ
