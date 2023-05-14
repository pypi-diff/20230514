# Comparing `tmp/noaawc-0.1.2.1-py3-none-any.whl.zip` & `tmp/noaawc-0.1.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 12311 bytes, number of entries: 19
+Zip file size: 12491 bytes, number of entries: 19
 -rw-rw-r--  2.0 unx       87 b- defN 23-Jan-14 01:52 noaawc/__init__.py
--rw-rw-r--  2.0 unx     4075 b- defN 23-Jan-29 03:08 noaawc/animate.py
+-rw-rw-r--  2.0 unx     4685 b- defN 23-May-14 07:00 noaawc/animate.py
 -rw-rw-r--  2.0 unx      217 b- defN 23-Jan-07 02:57 noaawc/main.py
--rw-rw-r--  2.0 unx     8857 b- defN 23-Jan-29 04:06 noaawc/plot.py
+-rw-rw-r--  2.0 unx     8991 b- defN 23-Apr-09 05:01 noaawc/plot.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jan-27 23:34 tests/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jan-14 13:07 tests/plot_gif.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jan-14 13:07 tests/plot_global.py
 -rw-rw-r--  2.0 unx      621 b- defN 23-Jan-27 23:29 tests/test_gif_surface_temp_zoom_focus_loc.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jan-27 23:34 tests/surface_temp/__init__.py
 -rw-rw-r--  2.0 unx      661 b- defN 23-Jan-27 23:33 tests/surface_temp/test_gif_surface_temp_spin.py
 -rw-rw-r--  2.0 unx      510 b- defN 23-Jan-27 23:33 tests/surface_temp/test_gif_surface_temp_zoom_focus.py
 -rw-rw-r--  2.0 unx      564 b- defN 23-Jan-27 23:32 tests/surface_temp/test_gif_surface_temp_zoom_focus_loc.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jan-27 23:30 tests/wind_temp/__init__.py
 -rw-rw-r--  2.0 unx      522 b- defN 23-Jan-27 23:30 tests/wind_temp/test_gif_wind_temp.py
--rw-rw-r--  2.0 unx     1067 b- defN 23-Jan-29 04:45 noaawc-0.1.2.1.dist-info/LICENSE
--rw-rw-r--  2.0 unx     8312 b- defN 23-Jan-29 04:45 noaawc-0.1.2.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jan-29 04:45 noaawc-0.1.2.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       13 b- defN 23-Jan-29 04:45 noaawc-0.1.2.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1582 b- defN 23-Jan-29 04:45 noaawc-0.1.2.1.dist-info/RECORD
-19 files, 27180 bytes uncompressed, 9685 bytes compressed:  64.4%
+-rw-rw-r--  2.0 unx     1067 b- defN 23-May-14 07:01 noaawc-0.1.5.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     8337 b- defN 23-May-14 07:01 noaawc-0.1.5.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-14 07:01 noaawc-0.1.5.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       13 b- defN 23-May-14 07:01 noaawc-0.1.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1572 b- defN 23-May-14 07:01 noaawc-0.1.5.dist-info/RECORD
+19 files, 27939 bytes uncompressed, 9885 bytes compressed:  64.6%
```

## zipnote {}

```diff
@@ -36,23 +36,23 @@
 
 Filename: tests/wind_temp/__init__.py
 Comment: 
 
 Filename: tests/wind_temp/test_gif_wind_temp.py
 Comment: 
 
-Filename: noaawc-0.1.2.1.dist-info/LICENSE
+Filename: noaawc-0.1.5.dist-info/LICENSE
 Comment: 
 
-Filename: noaawc-0.1.2.1.dist-info/METADATA
+Filename: noaawc-0.1.5.dist-info/METADATA
 Comment: 
 
-Filename: noaawc-0.1.2.1.dist-info/WHEEL
+Filename: noaawc-0.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: noaawc-0.1.2.1.dist-info/top_level.txt
+Filename: noaawc-0.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: noaawc-0.1.2.1.dist-info/RECORD
+Filename: noaawc-0.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## noaawc/animate.py

```diff
@@ -14,23 +14,27 @@
 import time
 import os
 from noaawc.plot import plot_global
 import matplotlib.pyplot as plt
 from noawclg.main import get_noaa_data as gnd
 from dataclasses import dataclass
 from kitano.logging import puts
+import statistics as stts
+import urllib
+from animateplot.video.video import RenderVideo
 
 global time0
 global ping_list
 time0=time.time()
 ping_list = [0]
+
 def ping_fun(ping_init:float,i,size):
     ping = time.time()-ping_init
-   # ping_list.append(ping)
-    ping_m = ping #sum(ping_list)/len(ping_list)
+    ping_list.append(ping)
+    ping_m = stts.median(ping_list) #sum(ping_list)/len(ping_list)
     i_=i+1
     eta = (size-i_)*ping_m
     min_eta = eta//60
     seg_eta = eta%60
     per = (i_/size)*100
     perr = time.time()-time0
     min_perr = perr//60
@@ -39,17 +43,18 @@
 
 
 
 
 @dataclass
 class Create_plot_gif:
     dn:gnd
-    path_save:str='img.gif'
+    path_gif:str='img.gif'
+    path_mp4:str='video.mp4'
     size:int=70
-    path_data:str='data/img_'
+    path_data:str='data'
     title:str=''
     key_noaa:str='vgrdpbl'
     loc_focus:tuple=(-9.45,-40.5)
     point_init=False
     point_end:float=False
     text_cb:str='°C'
     lon_stop:float=False
@@ -95,23 +100,24 @@
                 #print('before',lon_list)
             self.locs_focus = list(zip(self.lat_list,self.lon_list))
 
 
 
 
 
-    def render(self):
+    def render_cache(self):
         time_0=time.time()
 
-        if not os.path.isdir('data'):
-            os.mkdir('data')
+        if not os.path.isdir(self.path_data):
+            os.mkdir(self.path_data)
 
-        images = []          
+        images = []
+        img_path = urllib.parse.quote(self.title)
         for i in range(self.size):
-            path_img = f'{self.path_data}_{i}.png'
+            path_img = f'{self.path_data}/{img_path}_{i}.png'
 
             pg = plot_global(dn=self.dn,path=path_img,title=self.title,key_noaa=self.key_noaa,alpha=self.alpha,
                     indice=i,loc_focus=self.locs_focus[i],subtr_data=self.subtr_data,author=self.author,text_cb=self.text_cb)
 
             if self.zoom:
                 pg.zoom(*self.zoom)
                 
@@ -122,12 +128,29 @@
                 pg.annotate_data_loc(self.annotate_loc_txt,loc=self.annotate_loc_pos,color=self.color_annote_loc)
 
             pg.cmap = self.cmap
 
             pg.render(show=False)
             ping_fun(time_0,i,self.size)
             images.append(imageio.imread(path_img))
+        self.images = images
+
+
+
+
+    def render_gif(self):
+        print('rendering gif...')
+        path_gif = self.path_gif
+        imageio.mimsave(path_gif,self.images,fps=self.fps)
+        #for img in self.images:
+        os.system(f'rm -rf {self.path_data}/*.png')
+
+
+
+    def render_mp4(self,path_save:str):
+        print('rendering mp4...')
+        file_mp4 = path_save
+        render_video = RenderVideo(self.path_data,fps=self.fps)
+        render_video.render_mp4(file_mp4)
+        #for img in self.images:
+        os.system(f'rm -rf {self.path_data}/*.png')
 
-        print('criando gif...')
-        path_gif = self.path_save
-        imageio.mimsave(path_gif,images,fps=self.fps)
-        os.system('rm -rf data/*.png')
```

## noaawc/plot.py

```diff
@@ -29,14 +29,15 @@
 #         dn = gnd(date=yesterday)
 
 #keys = dn.get_noaa_keys()
 '''
 the function base and more
 important from it work
 '''
+
 plt.style.use('dark_background')
 
 @dataclass
 class plot_global:
     dn:gnd
     path:str='plot.png'
     indice:int=0
@@ -53,22 +54,27 @@
     edgecolor_text:str='black'
     annotate_size:float=9
     annotate_color:str='white'
     loc_focus:tuple=(0,0)
     key_noaa:str='tmpmwl'
     subtr_data:str=273,
     text_cb:str='ºC'
-    alpha:int=.9
+    alpha:float=.9
     author:str='@gpftc_ | @reinanbr_'
     level_data:int=25
+    resolution:str='c'
     keys:str = ''
     fillcontinents_colors:str = ''
     cmap:plt.cm = plt.cm.inferno
     ax:plt.subplot = plt.subplot(111)
     plt:plt=plt
+    
+    line_states:float=0.1
+    line_countries:float=0.35
+    
     xleft:int=None
     xright:int=None
     yup:int=None
     ydown:int=None
     
     annotate_pos_focus:tuple=None
     annotate_text_focus:str = None
@@ -115,15 +121,15 @@
             self.yup = yup*decai
             self.ydown = ydown*decai
 
     def rendering_image(self):
         self.m = Basemap(projection='ortho',
                          lat_0=self.loc_focus[0],
                          lon_0=self.loc_focus[1],
-                         resolution='c',llcrnrx=self.xleft, llcrnry=self.ydown, urcrnrx=self.xright, urcrnry=self.yup, 
+                         resolution=self.resolution,llcrnrx=self.xleft, llcrnry=self.ydown, urcrnrx=self.xright, urcrnry=self.yup, 
 )
         #self.m.bluemarble(scale=.5)
         
         self.x, self.y = self.m(*np.meshgrid(self.lon,self.lat))
         
         self.m.fillcontinents(self.fillcontinents_colors['color'],
                              self.fillcontinents_colors['lake_color'])
@@ -135,16 +141,16 @@
         #cm1=plt.contourf(x,y,data1,100,shading='nearest',cmap=plt.get_cmap('inferno'))
         #plt.cla()
         #plt.clf()
         self.cbar=self.plt.colorbar(self.cm,orientation='horizontal',extend='both',fraction=0.07,pad=0.05)
         #self.m.bluemarble()
         self.m.drawcoastlines()
         #self.m.drawmapboundary()#fill_color='aqua')
-        self.m.drawstates(linewidth=0.1)
-        self.m.drawcountries(linewidth=0.35)
+        self.m.drawstates(linewidth=self.line_states)
+        self.m.drawcountries(linewidth=self.line_countries)
         #self.m.drawcountries(linewidth=0.25)
         
         #m.drawmapboundary(fill_color='aqua')
 
         self.m.drawmeridians(np.arange(0,360,30))
         self.m.drawparallels(np.arange(-90,90,30))
         #print(dir(m))
@@ -153,21 +159,21 @@
     
     
     def rendering_text(self):
         self.cbar.set_label(self.text_cb,y=0,ha='right',color='white')
         self.cbar.ax.set_title(f'by: {self.author}',fontweight='bold')
         
         #xn2,yn2=m(-9.52,-40.61)
-        self.t = self.plt.text(-0.3,0.99,self.date_text, transform=self.ax.transAxes,
+        self.t = self.plt.text(-0.34,0.99,self.date_text, transform=self.ax.transAxes,
                     color='white', fontweight='bold',fontsize=14)
-        self.t = self.plt.text(1.1,1,f'*\n{self.key_noaa}:\n{self.keys[self.key_noaa]}',transform=self.ax.transAxes,
+        self.t = self.plt.text(1.16,1,f'*\n{self.key_noaa}:\n{self.keys[self.key_noaa]}',transform=self.ax.transAxes,
                     color='grey', fontweight='bold',fontsize=5)
-        self.t = self.plt.text(1.1,0.03,'data: GFS 0.25', transform=self.ax.transAxes,
+        self.t = self.plt.text(1.16,0.03,'data: GFS 0.25', transform=self.ax.transAxes,
                     color='white', fontweight='bold',fontsize=8)
-        self.t = self.plt.text(1.12,-0.01,'NOAA/NASA', transform=self.ax.transAxes,
+        self.t = self.plt.text(1.18,-0.01,'NOAA/NASA', transform=self.ax.transAxes,
                     color='grey', fontweight='bold',fontsize=8)
         #t.set_bbox(dict(facecolor='red', alpha=0.81, edgecolor='black'))
         
         if self.pos_text and self.text:
             self.t = self.plt.text(self.pos_text[0],self.pos_text[1], self.text, transform=self.ax.transAxes,
                         color=self.text_color, fontweight='bold',fontsize=self.text_size)
             self.t.set_bbox(dict(facecolor='red', alpha=0.81, edgecolor='black'))
@@ -236,8 +242,7 @@
         #    puts('saved plot')
         if show:
             self.plt.show()
         self.plt.cla()
         self.plt.clf()
 
 
-
```

## Comparing `noaawc-0.1.2.1.dist-info/LICENSE` & `noaawc-0.1.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `noaawc-0.1.2.1.dist-info/METADATA` & `noaawc-0.1.5.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: noaawc
-Version: 0.1.2.1
+Version: 0.1.5
 Summary: Library for plotting dataset from noaa site in basemap
 Home-page: https://github.com/reinanbr/noaawc
 Author: Reinan Br
 Author-email: slimchatuba@gmail.com
 License: GPLv3
 Keywords: climate weather noaa plots
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pygrib
 Requires-Dist: kitano
 Requires-Dist: numpy
 Requires-Dist: noawclg
 Requires-Dist: matplotlib
 Requires-Dist: pandas
+Requires-Dist: animateplot
 Requires-Dist: psutil
 Requires-Dist: imageio
 Requires-Dist: basemap
 
 
 <h1 align='center'></h1>
 <p align='center'>
```

## Comparing `noaawc-0.1.2.1.dist-info/RECORD` & `noaawc-0.1.5.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 noaawc/__init__.py,sha256=lgikjx-qPyvHx-w1VgjDB_i1x0pu1s_hZbTUEWCZIr8,87
-noaawc/animate.py,sha256=yzNkjJy4gMeHxEE8E9GMO_EPegoVPUtITZ-z8d7nAoM,4075
+noaawc/animate.py,sha256=zN6YxmvbPgkQxcednkRvdZqz7XthyEg7UfgySbAiorU,4685
 noaawc/main.py,sha256=zX8ZznAKADJVNcVKGArCG4exoKE_GlNRuKsFg5sGUeo,217
-noaawc/plot.py,sha256=eTE5Z28WcDzobFR9PsmhGPN3VWNc8vqiBa0nRPqwjSI,8857
+noaawc/plot.py,sha256=d7ZUvUyhEZJS0MBEsQdDAO3a_4eh6oFeR-ZQhSZp4TY,8991
 tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/plot_gif.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/plot_global.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/test_gif_surface_temp_zoom_focus_loc.py,sha256=eTUn1RlcWsDiaJH1JB1Qh5pbUZEQIQcOBMt5aVwzTuc,621
 tests/surface_temp/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/surface_temp/test_gif_surface_temp_spin.py,sha256=cTnH9Qt1Gw0uNjAJIL0xKKCu7xuE2T6E3ZXknx9ZYNA,661
 tests/surface_temp/test_gif_surface_temp_zoom_focus.py,sha256=Df-2X1oJGq_WN24Nn1KJKr2G-cBBbIQ6rSFc8PBXuCM,510
 tests/surface_temp/test_gif_surface_temp_zoom_focus_loc.py,sha256=gsndQBGEADVurUwpT172gYIRO5j9MtSIhFUneaQ9KGs,564
 tests/wind_temp/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/wind_temp/test_gif_wind_temp.py,sha256=NhvxdLrQnnaMjs1OgLfnkduxCSRQOEJe4ksW7horN2o,522
-noaawc-0.1.2.1.dist-info/LICENSE,sha256=3-GlIEVU7asdPr6aCmtazGIYHEDRxVWTOUBC9LzwAFI,1067
-noaawc-0.1.2.1.dist-info/METADATA,sha256=8t-cklgpsQujQCjFUKBpLEpv7JaKDyId6m53q1WVRDE,8312
-noaawc-0.1.2.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-noaawc-0.1.2.1.dist-info/top_level.txt,sha256=vFvCLni0J6LDgJmd6nhdE66ENT2gW6Lt2J1spa3IYPs,13
-noaawc-0.1.2.1.dist-info/RECORD,,
+noaawc-0.1.5.dist-info/LICENSE,sha256=3-GlIEVU7asdPr6aCmtazGIYHEDRxVWTOUBC9LzwAFI,1067
+noaawc-0.1.5.dist-info/METADATA,sha256=FR8uMidUUbtgR41aJgcx15dDFCFvzfSCynMyVmuIb_Q,8337
+noaawc-0.1.5.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+noaawc-0.1.5.dist-info/top_level.txt,sha256=vFvCLni0J6LDgJmd6nhdE66ENT2gW6Lt2J1spa3IYPs,13
+noaawc-0.1.5.dist-info/RECORD,,
```

