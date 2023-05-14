# Comparing `tmp/pyapep-0.1.0.tar.gz` & `tmp/pyapep-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyapep-0.1.0.tar", last modified: Mon Apr 10 12:53:37 2023, max compression
+gzip compressed data, was "pyapep-0.1.2.tar", last modified: Sun May 14 14:42:15 2023, max compression
```

## Comparing `pyapep-0.1.0.tar` & `pyapep-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 12:53:37.013400 pyapep-0.1.0/
--rw-rw-rw-   0        0        0      352 2023-04-10 12:53:37.012387 pyapep-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      367 2022-05-27 15:52:19.000000 pyapep-0.1.0/README
-drwxrwxrwx   0        0        0        0 2023-04-10 12:53:36.969858 pyapep-0.1.0/pyapep/
--rw-rw-rw-   0        0        0        0 2022-10-19 06:19:02.000000 pyapep-0.1.0/pyapep/__init__.py
--rw-rw-rw-   0        0        0    22187 2022-12-20 03:37:29.000000 pyapep-0.1.0/pyapep/isofit.py
--rw-rw-rw-   0        0        0     8353 2022-05-27 15:52:19.000000 pyapep-0.1.0/pyapep/simide.py
--rw-rw-rw-   0        0        0    90223 2022-10-19 06:19:02.000000 pyapep-0.1.0/pyapep/simsep.py
--rw-rw-rw-   0        0        0    87603 2022-10-19 06:19:02.000000 pyapep-0.1.0/pyapep/simsep_backup.py
-drwxrwxrwx   0        0        0        0 2023-04-10 12:53:37.009477 pyapep-0.1.0/pyapep.egg-info/
--rw-rw-rw-   0        0        0      352 2023-04-10 12:53:35.000000 pyapep-0.1.0/pyapep.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-04-10 12:53:36.000000 pyapep-0.1.0/pyapep.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 12:53:35.000000 pyapep-0.1.0/pyapep.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-04-10 12:53:36.000000 pyapep-0.1.0/pyapep.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-10 12:53:36.000000 pyapep-0.1.0/pyapep.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 12:53:37.014405 pyapep-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      931 2023-04-10 12:52:58.000000 pyapep-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:42:15.107047 pyapep-0.1.2/
+-rw-rw-rw-   0        0        0      352 2023-05-14 14:42:15.107047 pyapep-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      367 2022-05-27 15:52:19.000000 pyapep-0.1.2/README
+drwxrwxrwx   0        0        0        0 2023-05-14 14:42:15.107047 pyapep-0.1.2/pyapep/
+-rw-rw-rw-   0        0        0        0 2022-10-19 06:19:02.000000 pyapep-0.1.2/pyapep/__init__.py
+-rw-rw-rw-   0        0        0    22187 2022-12-20 03:37:29.000000 pyapep-0.1.2/pyapep/isofit.py
+-rw-rw-rw-   0        0        0     8353 2022-05-27 15:52:19.000000 pyapep-0.1.2/pyapep/simide.py
+-rw-rw-rw-   0        0        0   116098 2023-05-13 11:52:01.000000 pyapep-0.1.2/pyapep/simsep.py
+-rw-rw-rw-   0        0        0    87603 2022-10-19 06:19:02.000000 pyapep-0.1.2/pyapep/simsep_backup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:42:15.107047 pyapep-0.1.2/pyapep.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-05-14 14:42:13.000000 pyapep-0.1.2/pyapep.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-05-14 14:42:14.000000 pyapep-0.1.2/pyapep.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 14:42:13.000000 pyapep-0.1.2/pyapep.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-05-14 14:42:14.000000 pyapep-0.1.2/pyapep.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-14 14:42:14.000000 pyapep-0.1.2/pyapep.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-14 14:42:15.122571 pyapep-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      931 2023-05-14 14:41:22.000000 pyapep-0.1.2/setup.py
```

### Comparing `pyapep-0.1.0/pyapep/isofit.py` & `pyapep-0.1.2/pyapep/isofit.py`

 * *Files identical despite different names*

### Comparing `pyapep-0.1.0/pyapep/simide.py` & `pyapep-0.1.2/pyapep/simide.py`

 * *Files identical despite different names*

### Comparing `pyapep-0.1.0/pyapep/simsep.py` & `pyapep-0.1.2/pyapep/simsep_backup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 # %% Import packages
 import numpy as np
 #from numpy.lib.function_base import _parse_input_dimensions
-from scipy.integrate import odeint, solve_ivp
+from scipy.integrate import odeint
 import matplotlib.pyplot as plt
 import time
 from scipy.interpolate import interp1d
 from scipy.integrate import solve_ivp
  
 # %% Global varaiebls
 R_gas = 8.3145      # 8.3145 J/mol/K
@@ -15,43 +15,31 @@
 def Ergun(C_array,T_array, M_molar, mu_vis, D_particle,epsi_void,d,dd,d_fo, N):
     rho_g = np.zeros(N)
     for c, m in zip(C_array, M_molar):
         rho_g = rho_g + m*c
     P = np.zeros(N)
     for cc in C_array: 
         P = P + cc*R_gas*T_array
-    dP = d_fo@P
-    #ddP = dd@P
-
+    dP = d@P
+    
     Vs_Vg = (1-epsi_void)/epsi_void
     A =1.75*rho_g/D_particle*Vs_Vg
     B = 150*mu_vis/D_particle**2*Vs_Vg**2
     C = dP
  
     ind_posi = B**2-4*A*C >= 0
     ind_nega = ind_posi == False
     v_pos = (-B[ind_posi]+ np.sqrt(B[ind_posi]**2-4*A[ind_posi]*C[ind_posi]))/(2*A[ind_posi])
     v_neg = (B[ind_nega] - np.sqrt(B[ind_nega]**2+4*A[ind_nega]*C[ind_nega]))/(2*A[ind_nega])
-    # v_neg = 0 
+    
     v_return = np.zeros(N)
     v_return[ind_posi] = v_pos
     v_return[ind_nega] = v_neg
-
-    #AA = -ddP/Vs_Vg
-    #BB = 3.5*rho_g/D_particle*v_return
-    #CC = 150*mu_vis/D_particle**2
-    #dv_pos = AA[ind_posi]/(BB[ind_posi]+CC[ind_posi])
-    #dv_neg = AA[ind_nega]/(BB[ind_nega]-CC[ind_nega])
-    # dv_pos = -epsi_void*ddP[ind_posi]/(3.5*rho_g[ind_posi]/D_particle*v_return[ind_posi]+150*mu_vis[ind_posi]/D_particle**2)/(1-epsi_void)
-    
-    # dv_neg = -epsi_void*ddP[ind_nega]/(3.5*rho_g[ind_nega]/D_particle*v_return[ind_nega]-150*mu_vis[ind_posi]/D_particle**2)/(1-epsi_void)
-    # dv_return = np.zeros(N)
-    # dv_return[ind_posi] = dv_pos
-    # dv_return[ind_nega] = dv_neg
-    dv_return = d@v_return
+    
+    dv_return = d_fo@v_return
     return v_return, dv_return
 
 def Ergun_test(dP,M_molar, mu_vis, D_particle,epsi_void):
     rho_g = 40*M_molar
     Vs_Vg = (1-epsi_void)/epsi_void
     A =1.75*rho_g/D_particle*Vs_Vg*np.ones_like(dP)
     B = 150*mu_vis/D_particle**2*Vs_Vg**2*np.ones_like(dP)
@@ -73,32 +61,28 @@
     if isinstance(y_raw,list):
         fn_list = []
         y_return = []
         z_new = np.linspace(z_raw[0], z_raw[-1],N_new)
         for yr in y_raw:
             fn_tmp = interp1d(z_raw,yr)
             y_new_tmp = fn_tmp(z_new)
-            y_new_tmp[y_new_tmp < 0] = 0
             y_return.append(y_new_tmp)
     elif len(y_raw.shape) == 1:
         yy = y_raw
         fn_tmp = interp1d(z_raw, yy, kind = 'cubic')
         z_new = np.linspace(z_raw[0], z_raw[-1],N_new)
         y_return = fn_tmp(z_new)
-        y_return[y_return < 0] = 0
     elif len(y_raw.shape) == 2:
         yy = y_raw[-1,:]
         fn_tmp = interp1d(z_raw, yy, kind = 'cubic')
         z_new = np.linspace(z_raw[0], z_raw[-1],N_new)
         y_return = fn_tmp(z_new)
-        y_return[y_return < 0] = 0
     else:
         print('Input should be 1d or 2d array.')
         return None
-    
     return y_return
 
 # %% Column class
 class column:
     def __init__(self, L, A_cross, n_component, 
                  N_node = 11, E_balance = True):
         self._L = L
@@ -346,17 +330,17 @@
             T = self._Tg_init
             for ii in range(n_comp):
                 dC.append(self._d@C[ii])
                 ddC.append(self._dd@C[ii])
                 P_part.append(C[ii]*R_gas*T/1E5) # in bar
                 C_ov = C_ov + C[ii]
                 P_ov = P_ov + C[ii]*R_gas*T
-                Mu = Mu + C[ii]*self._mu[ii]
+                Mu = C[ii]*self._mu[ii]
             Mu = Mu/C_ov
-            #Mu = np.mean(self._mu)*np.ones_like(self._N)
+
             # Ergun equation
             v,dv = Ergun(C,T,self._M_m,Mu,self._D_p,epsi,
                          self._d,self._dd,self._d_fo, self._N)
             
             # Solid phase
             qsta = self._iso(P_part, T) # partial pressure in bar
             dqdt = []
@@ -380,28 +364,16 @@
             h = self._h
             # Gas phase
             dCdt = []
             for ii in range(n_comp):
                 dCdt_tmp = -v*dC[ii] -C[ii]*dv + D_dis[ii]*ddC[ii] - (1-epsi)/epsi*rho_s*dqdt[ii]
                 #dCdt_tmp[0] = +(v_in*C_sta[ii] - v[1]*C[ii][0])/h - (1-epsi)/epsi*rho_s*dqdt[ii][0]
                 #dCdt_tmp[-1]= +(v[-1]*C[ii][-2]- v_out*C[ii][-1])/h - (1-epsi)/epsi*rho_s*dqdt[ii][-1]
-                #dCdt_tmp[0] = v_in*(C_sta[ii]-C[ii][0])/h- (1-epsi)/epsi*rho_s*dqdt[ii][0]
-                #dCdt_tmp[-1]= +(v_out+v[-1])/2*(C[ii][-2]- C[ii][-1])/h - (1-epsi)/epsi*rho_s*dqdt[ii][-1]
-                dCdt_tmp[0] = (v_in*C_sta[ii]-v[0]*C[ii][0])/h- (1-epsi)/epsi*rho_s*dqdt[ii][0]
-                dCdt_tmp[-1]= +(v[-2]*C[ii][-2]- v_out*C[ii][-1])/h - (1-epsi)/epsi*rho_s*dqdt[ii][-1]
-###################################################3
-#                dv0 = (v[0] - v_in)/h
-#                dC0 = (C[ii][0] - C_sta[ii])/h
-#
-#                dvL = (v_out-v[-2])/h
-#                dCL = (C[ii][-1] - C[ii][-2])/h
-#                dCdt_tmp[0] = -v[0]*dC0 - C[ii][0]*dv0 - (1-epsi)/epsi*rho_s*dqdt[ii][0]
-#                dCdt_tmp[-1]= -v_out*dCL-C[ii][-1]*dvL - (1-epsi)/epsi*rho_s*dqdt[ii][-1]
-###################################################3
-
+                dCdt_tmp[0] = v_in*(C_sta[ii]-C[ii][0])/h- (1-epsi)/epsi*rho_s*dqdt[ii][0]
+                dCdt_tmp[-1]= +(v_out+v[-1])/2*(C[ii][-2]- C[ii][-1])/h - (1-epsi)/epsi*rho_s*dqdt[ii][-1]
                 dCdt.append(dCdt_tmp)
  
             dydt_tmp = dCdt+dqdt
             dydt = np.concatenate(dydt_tmp)
             return dydt
         
         C_init = []
@@ -509,15 +481,15 @@
             # Viscosity
             for ii in range(n_comp):
                 dC.append(self._d@C[ii])
                 ddC.append(self._dd@C[ii])
                 P_part.append(C[ii]*R_gas*Tg/1E5) # in bar
                 C_ov = C_ov + C[ii]
                 P_ov = P_ov + C[ii]*R_gas*Tg
-                Mu = Mu + C[ii]*self._mu[ii]
+                Mu = C[ii]*self._mu[ii]
             Mu = Mu/C_ov
 
             # Ergun equation
             v,dv = Ergun(C,Tg,self._M_m,Mu,self._D_p,epsi,
                          self._d,self._dd,self._d_fo, self._N)
             
             # Solid phase concentration
@@ -540,18 +512,16 @@
             v_out = max(self._Cv_out*(P_ov[-1]/1E5 - self._P_out), 0 )  # pressure in bar
             
             # Gas phase concentration
             dCdt = []
             for ii in range(n_comp):
                 dCdt_tmp = -v*dC[ii] -C[ii]*dv + D_dis[ii]*ddC[ii] - (1-epsi)/epsi*rho_s*dqdt[ii]
                 #dCdt_tmp[0] = +(v_in*C_sta[ii] - v[1]*C[ii][0])/h - (1-epsi)/epsi*rho_s*dqdt[ii][0]    
-                #dCdt_tmp[0] = +v_in*(C_sta[ii] - C[ii][0])/h - (1-epsi)/epsi*rho_s*dqdt[ii][0]
-                #dCdt_tmp[-1]= +(v_out+v[-1])/2*(C[ii][-2]- C[ii][-1])/h - (1-epsi)/epsi*rho_s*dqdt[ii][-1]
-                dCdt_tmp[0] = (v_in*C_sta[ii]-v[0]*C[ii][0])/h- (1-epsi)/epsi*rho_s*dqdt[ii][0]
-                dCdt_tmp[-1]= +(v[-2]*C[ii][-2]- v_out*C[ii][-1])/h - (1-epsi)/epsi*rho_s*dqdt[ii][-1]
+                dCdt_tmp[0] = +v_in*(C_sta[ii] - C[ii][0])/h - (1-epsi)/epsi*rho_s*dqdt[ii][0]
+                dCdt_tmp[-1]= +(v_out+v[-1])/2*(C[ii][-2]- C[ii][-1])/h - (1-epsi)/epsi*rho_s*dqdt[ii][-1]
                 dCdt.append(dCdt_tmp)
             # Temperature (gas)
             Cov_Cpg = np.zeros(N) # Heat capacity (overall) J/K/m^3
             for ii in range(n_comp):
                 Cov_Cpg = Cov_Cpg + Cpg[ii]*C[ii]
             dTgdt = -v*dTg + h_heat*a_surf/epsi*(Ts - Tg)/Cov_Cpg
             for ii in range(n_comp):
@@ -649,15 +619,15 @@
 
         C_sta = []
         Cov_Cpg_in = 0
         for ii in range(n_comp):
             C_sta.append(self._y_in[ii]*self._P_in/R_gas/self._T_in*1E5)
             Cov_Cpg_in = Cov_Cpg_in + Cpg[ii]*C_sta[ii]
         
-        def massmomeenerbal(y, t):
+        def massmomeenerbal(y,t):
             C = []
             q = []
             for ii in range(n_comp):
                 C.append(y[ii*N:(ii+1)*N])
                 q.append(y[n_comp*N + ii*N : n_comp*N + (ii+1)*N])
             Tg = y[2*n_comp*N : 2*n_comp*N + N ]
             Ts = y[2*n_comp*N + N : 2*n_comp*N + 2*N ]
@@ -680,17 +650,16 @@
             # Viscosity
             for ii in range(n_comp):
                 dC.append(self._d@C[ii])
                 ddC.append(self._dd@C[ii])
                 P_part.append(C[ii]*R_gas*Tg/1E5) # in bar
                 C_ov = C_ov + C[ii]
                 P_ov = P_ov + C[ii]*R_gas*Tg
-                Mu = Mu + C[ii]*self._mu[ii]
+                Mu = C[ii]*self._mu[ii]
             Mu = Mu/C_ov
-             
 
             # Ergun equation
             v,dv = Ergun(C,Tg,self._M_m,Mu,self._D_p,epsi,
                          self._d,self._dd,self._d_fo, self._N)
             
             # Solid phase concentration
             qsta = self._iso(P_part, Tg) # partial pressure in bar
@@ -705,51 +674,39 @@
                     dqdt.append(dqdt_tmp)
             # Valve equations (v_in and v_out)
             #P_in = (C1_sta + C2_sta)*R_gas*T_gas
             if self._const_v:
                 v_in = self._Q_in/epsi/self._A
             else:
                 v_in = max(self._Cv_in*(self._P_in - P_ov[0]/1E5), 0 )  # pressure in bar           
-                v_in = self._Cv_in*(self._P_in - P_ov[0]/1E5)  # pressure in bar           
             v_out = max(self._Cv_out*(P_ov[-1]/1E5 - self._P_out), 0 )  # pressure in bar
             
             # Gas phase concentration
             dCdt = []
             for ii in range(n_comp):
                 dCdt_tmp = -v*dC[ii] -C[ii]*dv + D_dis[ii]*ddC[ii] - (1-epsi)/epsi*rho_s*dqdt[ii]
-                #dCdt_tmp[0] = +(v_in*C_sta[ii] - v[1]*C[ii][0])/h - (1-epsi)/epsi*rho_s*dqdt[ii][0]    
+                dCdt_tmp[0] = +(v_in*C_sta[ii] - v[1]*C[ii][0])/h - (1-epsi)/epsi*rho_s*dqdt[ii][0]    
                 #dCdt_tmp[0] = +(v_in*C_sta[ii] - v[1]*C[ii][0])/h - (1-epsi)/epsi*rho_s*dqdt[ii][0]
-                #dCdt_tmp[-1]= +(v[-1]*C[ii][-2]- v_out*C[ii][-1])/h - (1-epsi)/epsi*rho_s*dqdt[ii][-1]
-                dCdt_tmp[0] = (v_in*C_sta[ii]-v[0]*C[ii][0])/h- (1-epsi)/epsi*rho_s*dqdt[ii][0]
-                dCdt_tmp[-1]= +(v[-2]*C[ii][-2]- v_out*C[ii][-1])/h - (1-epsi)/epsi*rho_s*dqdt[ii][-1]
-###################################################3
-                dv0 = (v[0] - v_in)/h
-                dC0 = (C[ii][0] - C_sta[ii])/h
-
-                dvL = (v_out-v[-2])/h
-                dCL = (C[ii][-1] - C[ii][-2])/h
-                dCdt_tmp[0] = -v[0]*dC0 - C[ii][0]*dv0 - (1-epsi)/epsi*rho_s*dqdt[ii][0]
-                dCdt_tmp[-1]= -v_out*dCL-C[ii][-1]*dvL - (1-epsi)/epsi*rho_s*dqdt[ii][-1]
-###################################################3
+                dCdt_tmp[-1]= +(v[-1]*C[ii][-2]- v_out*C[ii][-1])/h - (1-epsi)/epsi*rho_s*dqdt[ii][-1]
                 dCdt.append(dCdt_tmp)
             # Temperature (gas)
             Cov_Cpg = np.zeros(N) # Heat capacity (overall) J/K/m^3
             for ii in range(n_comp):
                 Cov_Cpg = Cov_Cpg + Cpg[ii]*C[ii]
             dTgdt = -v*dTg + h_heat*a_surf/epsi*(Ts - Tg)/Cov_Cpg
             for ii in range(n_comp):
                 dTgdt = dTgdt - Cpg[ii]*Tg*D_dis[ii]*ddC[ii]/Cov_Cpg
                 dTgdt = dTgdt + Tg*self._rho_s*(1-epsi)/epsi*Cpg[ii]*dqdt[ii]/Cov_Cpg
                 dTgdt = dTgdt + h_ambi*4/epsi/D_col*(T_ambi - Tg)/Cov_Cpg
 
             dTgdt[0] = h_heat*a_surf/epsi*(Ts[0] - Tg[0])/Cov_Cpg[0]
-            dTgdt[0] = dTgdt[0] + (v_in*self._T_in*Cov_Cpg_in/Cov_Cpg[0] - v[0]*Tg[0])/h
+            dTgdt[0] = dTgdt[0] + (v_in*self._T_in*Cov_Cpg_in/Cov_Cpg[0] - v[1]*Tg[0])/h
             dTgdt[-1] = h_heat*a_surf/epsi*(Ts[-1] - Tg[-1])/Cov_Cpg[-1]
             #dTgdt[-1] = dTgdt[-1] + (v[-1]*Tg[-2]*Cov_Cpg[-2]/Cov_Cpg[-1] - v_out*Tg[-1])/h
-            dTgdt[-1] = dTgdt[-1] + (v[-2]*Tg[-2]*Cov_Cpg[-2]/Cov_Cpg[-1] - v_out*Tg[-1])/h
+            dTgdt[-1] = dTgdt[-1] + (v[-1]*Tg[-2]*Cov_Cpg[-2]/Cov_Cpg[-1] - v_out*Tg[-1])/h
             for ii in range(n_comp):
                 dTgdt[0] = dTgdt[0] - Tg[0]*Cpg[ii]*dCdt[ii][0]/Cov_Cpg[0]
                 dTgdt[-1] = dTgdt[-1] - Tg[-1]*Cpg[ii]*dCdt[ii][-1]/Cov_Cpg[-1]
             dTsdt = (self._k_cond*ddTs+ h_heat*a_surf/(1-epsi)*(Tg-Ts))/self._rho_s/Cps
             for ii in range(n_comp):
                 dTsdt = dTsdt + abs(dH[ii])*dqdt[ii]/Cps
             
@@ -772,29 +729,27 @@
                 q_init[ii] = self._A_flip@q_init[ii]
             y0_tmp = C_init + q_init + [self._A_flip@self._Tg_init] + [self._A_flip@self._Ts_init]
         else:
             y0_tmp = C_init + q_init + [self._Tg_init] + [self._Ts_init]
         y0 = np.concatenate(y0_tmp)
         
         #RUN
-        y_result = odeint(massmomeenerbal,y0, t_dom,)
-        #y_ivp = solve_ivp(massmomeenerbal,t_dom, y0,method = 'BDF')
-        #y_result = y_ivp.y
+        y_result = odeint(massmomeenerbal,y0,t_dom,)
         C_sum = 0
         for ii in range(n_comp):
             C_sum = C_sum + y_result[-1,ii*N+2]
         if C_sum  < 0.1:
             y_result, _,_  = self.run_mamoen_alt(t_max,n_sec)
             toc = time.time()/60 - tic
             self._CPU_min = toc
             self._Tg_res = y_result[:,n_comp*2*N : n_comp*2*N+N]
             if CPUtime_print:
                 print('Simulation of this step is completed.')
                 print('This took {0:9.3f} mins to run. \n'.format(toc))
-            return y_result, self._z, t_dom
+            return y_result
         
         if self._required['Flow direction'] == 'Backward':
             y_tmp = []
             for ii in range(n_comp*2 + 2):
                 mat_tmp = y_result[:, ii*N : (ii+1)*N]
                 y_tmp.append(mat_tmp@self._A_flip)
             y_flip = np.concatenate(y_tmp, axis = 1)
@@ -1113,15 +1068,15 @@
     n_t = t_max_int*n_sec+ 1
     n_comp = column1._n_comp
     
     # Target pressure
     C_sta1 = np.zeros(n_comp)
     for ii in range(n_comp):
         C_sta1[ii] = c1_tmp._y_init[ii][0]*P_mean/R_gas/T_mean*1E5
-    #print(C_sta1)
+    print(C_sta1)
 
     t_dom = np.linspace(0,t_max_int, n_t)
     column1._n_sec = n_sec
     column2._n_sec = n_sec
     if t_max_int < t_max:
         t_dom = np.concatenate((t_dom, [t_max]))
 
@@ -2204,25 +2159,25 @@
         numor0 = isopar1[0]*b1*P[0]
         numor1 = isopar2[0]*b2*P[1]
         q_return = [numor0/denom, numor1/denom]
         return q_return
  
     epsi_test = 0.4         # macroscopic void fraction (m^3/m^3)
     D_particle_dia = 0.01   # particle diameter (m)
-    rho_s_test = 1100       # solid density (kg/m^3)
+    rho_s_test = 1100       # solid density (kg/mol)
     c1.adsorbent_info(iso_fn_test,epsi_test,D_particle_dia, rho_s_test)
  
     M_m_test  = [0.044, 0.028]      ## molar mass    (kg/mol)
     mu_test = [1.47E-5, 1.74E-5]    ## gas viscosity (Pa sec)
     c1.gas_prop_info(M_m_test, mu_test)
  
     ## Mass transfer coefficients
     D_dis_test = [1E-6, 1E-6]   # m^2/sec
     k_MTC = [0.0002, 0.0002]    # m/sec
-    a_surf = 200                # m^2/m^3
+    a_surf = 400                # m^2/m^3
     c1.mass_trans_info(k_MTC, a_surf, D_dis_test)
 
     ## Thermal properties
     Del_H = [30E3, 20E3]    # J/mol
     Cp_s = 935              # J/kg/K
     Cp_g = [37.22, 29.15]   # J/mol/K
     h_heat = 100            # J/sec/m^2/K
@@ -2263,26 +2218,25 @@
     c2 = c1.copy()
     c1.next_init()
 
     c1.boundaryC_info(Pout_test,Pin_test,Tin_test,yin_test,
     0.0*Cvin_test,Cvout_test,Q_in_test,False, foward_flow_direction=True)
     c2.boundaryC_info(Pout_test,Pin_test,Tin_test,yin_test,
     0.0*Cvin_test,0,Q_in_test,False, foward_flow_direction=True)
-    '''
+
     step_P_eq(
         c1,c2,100,n_sec = 50,
         valve_select = [1,1],
         Cv_btw=0.05,CPUtime_print=True)
     plt.show()
     Legend_loc = [1.15, 0.9]
     c1.Graph_P(10, loc = Legend_loc)
     c1.Graph(10,2, loc =Legend_loc)
     c1.Graph(10,3, loc =Legend_loc)
     c2.Graph_P(10, loc =Legend_loc)
     c2.Graph(10,2, loc =Legend_loc)
     c2.Graph(10,3, loc = Legend_loc)
     plt.show( )
-    '''
     
 # %%
 
 # %%
```

### Comparing `pyapep-0.1.0/pyapep/simsep_backup.py` & `pyapep-0.1.2/pyapep/simsep.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,45 +1,57 @@
 
 # %% Import packages
 import numpy as np
 #from numpy.lib.function_base import _parse_input_dimensions
-from scipy.integrate import odeint
+from scipy.integrate import odeint, solve_ivp
 import matplotlib.pyplot as plt
 import time
 from scipy.interpolate import interp1d
-from scipy.integrate import solve_ivp
+#from scipy.integrate import solve_ivp
  
 # %% Global varaiebls
 R_gas = 8.3145      # 8.3145 J/mol/K
  
 # %% column (bed) class
 def Ergun(C_array,T_array, M_molar, mu_vis, D_particle,epsi_void,d,dd,d_fo, N):
     rho_g = np.zeros(N)
     for c, m in zip(C_array, M_molar):
         rho_g = rho_g + m*c
     P = np.zeros(N)
     for cc in C_array: 
         P = P + cc*R_gas*T_array
-    dP = d@P
-    
+    dP = d_fo@P
+    #ddP = dd@P
+
     Vs_Vg = (1-epsi_void)/epsi_void
     A =1.75*rho_g/D_particle*Vs_Vg
     B = 150*mu_vis/D_particle**2*Vs_Vg**2
     C = dP
  
     ind_posi = B**2-4*A*C >= 0
     ind_nega = ind_posi == False
     v_pos = (-B[ind_posi]+ np.sqrt(B[ind_posi]**2-4*A[ind_posi]*C[ind_posi]))/(2*A[ind_posi])
     v_neg = (B[ind_nega] - np.sqrt(B[ind_nega]**2+4*A[ind_nega]*C[ind_nega]))/(2*A[ind_nega])
-    
+    # v_neg = 0 
     v_return = np.zeros(N)
     v_return[ind_posi] = v_pos
     v_return[ind_nega] = v_neg
-    
-    dv_return = d_fo@v_return
+
+    #AA = -ddP/Vs_Vg
+    #BB = 3.5*rho_g/D_particle*v_return
+    #CC = 150*mu_vis/D_particle**2
+    #dv_pos = AA[ind_posi]/(BB[ind_posi]+CC[ind_posi])
+    #dv_neg = AA[ind_nega]/(BB[ind_nega]-CC[ind_nega])
+    # dv_pos = -epsi_void*ddP[ind_posi]/(3.5*rho_g[ind_posi]/D_particle*v_return[ind_posi]+150*mu_vis[ind_posi]/D_particle**2)/(1-epsi_void)
+    
+    # dv_neg = -epsi_void*ddP[ind_nega]/(3.5*rho_g[ind_nega]/D_particle*v_return[ind_nega]-150*mu_vis[ind_posi]/D_particle**2)/(1-epsi_void)
+    # dv_return = np.zeros(N)
+    # dv_return[ind_posi] = dv_pos
+    # dv_return[ind_nega] = dv_neg
+    dv_return = d@v_return
     return v_return, dv_return
 
 def Ergun_test(dP,M_molar, mu_vis, D_particle,epsi_void):
     rho_g = 40*M_molar
     Vs_Vg = (1-epsi_void)/epsi_void
     A =1.75*rho_g/D_particle*Vs_Vg*np.ones_like(dP)
     B = 150*mu_vis/D_particle**2*Vs_Vg**2*np.ones_like(dP)
@@ -61,30 +73,70 @@
     if isinstance(y_raw,list):
         fn_list = []
         y_return = []
         z_new = np.linspace(z_raw[0], z_raw[-1],N_new)
         for yr in y_raw:
             fn_tmp = interp1d(z_raw,yr)
             y_new_tmp = fn_tmp(z_new)
+            y_new_tmp[y_new_tmp < 0] = 0
             y_return.append(y_new_tmp)
     elif len(y_raw.shape) == 1:
         yy = y_raw
         fn_tmp = interp1d(z_raw, yy, kind = 'cubic')
         z_new = np.linspace(z_raw[0], z_raw[-1],N_new)
         y_return = fn_tmp(z_new)
+        y_return[y_return < 0] = 0
     elif len(y_raw.shape) == 2:
         yy = y_raw[-1,:]
         fn_tmp = interp1d(z_raw, yy, kind = 'cubic')
         z_new = np.linspace(z_raw[0], z_raw[-1],N_new)
         y_return = fn_tmp(z_new)
+        y_return[y_return < 0] = 0
     else:
         print('Input should be 1d or 2d array.')
         return None
+    
     return y_return
 
+# %% GaODE: NewODE function
+def gaode(dy_fun, y0, t, args= None):
+#    if np.isscalar(t):
+#        t_domain = np.linspace(0,t, 10001, dtype=np.float64)
+#    else:
+#        t_domain = np.array(t[:], dtype = np.float64)
+    t_domain = np.array(t[:], dtype = np.float64)
+    y_res = []
+    dt_arr = t_domain[1:] - t_domain[:-1]
+
+    N = len(y0)
+    tt_prev = t_domain[0]
+    y_tmp = np.array(y0, dtype = np.float64)
+    y_res.append(y_tmp)
+    if args == None:
+        for tt, dtt in zip(t_domain[:-1], dt_arr):
+            dy_tmp = dy_fun(y_tmp, tt)
+            y_tmp_new = y_tmp + dy_tmp*dtt
+            tt_prev = tt
+            y_res.append(y_tmp_new)
+            y_tmp = y_tmp_new
+#            if tt%10 == 1:
+#                print(y_tmp_new, y_tmp)
+        y_res_arr = np.array(y_res, dtype = np.float64)
+    else:
+        for tt, dtt in zip(t_domain[1:], dt_arr):
+            dy_tmp = dy_fun(y_tmp, tt, *args)
+            y_tmp_new = y_tmp + dy_tmp*dtt
+            tt_prev = tt
+            y_res.append(y_tmp_new)
+            y_tmp = y_tmp_new
+        y_res_arr = np.array(y_res, dtype=object)
+    
+    return y_res_arr
+
+
 # %% Column class
 class column:
     def __init__(self, L, A_cross, n_component, 
                  N_node = 11, E_balance = True):
         self._L = L
         self._A = A_cross
         self._n_comp = n_component
@@ -94,14 +146,15 @@
         'adsorbent_info':False,
         'gas_prop_info': False,
         'mass_trans_info': False,}
         if E_balance:
             self._required['thermal_info'] = False
         self._required['boundaryC_info'] = False
         self._required['initialC_info'] = False
+        self.is_BASIS = False
         h = L/(N_node-1)
         h_arr = h*np.ones(N_node)
         self._h = h
  
         # FDM backward, 1st deriv
         d0 = np.diag(1/h_arr, k = 0)
         d1 = np.diag(-1/h_arr[1:], k = -1)
@@ -330,17 +383,17 @@
             T = self._Tg_init
             for ii in range(n_comp):
                 dC.append(self._d@C[ii])
                 ddC.append(self._dd@C[ii])
                 P_part.append(C[ii]*R_gas*T/1E5) # in bar
                 C_ov = C_ov + C[ii]
                 P_ov = P_ov + C[ii]*R_gas*T
-                Mu = C[ii]*self._mu[ii]
+                Mu = Mu + C[ii]*self._mu[ii]
             Mu = Mu/C_ov
-
+            #Mu = np.mean(self._mu)*np.ones_like(self._N)
             # Ergun equation
             v,dv = Ergun(C,T,self._M_m,Mu,self._D_p,epsi,
                          self._d,self._dd,self._d_fo, self._N)
             
             # Solid phase
             qsta = self._iso(P_part, T) # partial pressure in bar
             dqdt = []
@@ -364,16 +417,28 @@
             h = self._h
             # Gas phase
             dCdt = []
             for ii in range(n_comp):
                 dCdt_tmp = -v*dC[ii] -C[ii]*dv + D_dis[ii]*ddC[ii] - (1-epsi)/epsi*rho_s*dqdt[ii]
                 #dCdt_tmp[0] = +(v_in*C_sta[ii] - v[1]*C[ii][0])/h - (1-epsi)/epsi*rho_s*dqdt[ii][0]
                 #dCdt_tmp[-1]= +(v[-1]*C[ii][-2]- v_out*C[ii][-1])/h - (1-epsi)/epsi*rho_s*dqdt[ii][-1]
-                dCdt_tmp[0] = v_in*(C_sta[ii]-C[ii][0])/h- (1-epsi)/epsi*rho_s*dqdt[ii][0]
-                dCdt_tmp[-1]= +(v_out+v[-1])/2*(C[ii][-2]- C[ii][-1])/h - (1-epsi)/epsi*rho_s*dqdt[ii][-1]
+                #dCdt_tmp[0] = v_in*(C_sta[ii]-C[ii][0])/h- (1-epsi)/epsi*rho_s*dqdt[ii][0]
+                #dCdt_tmp[-1]= +(v_out+v[-1])/2*(C[ii][-2]- C[ii][-1])/h - (1-epsi)/epsi*rho_s*dqdt[ii][-1]
+                dCdt_tmp[0] = (v_in*C_sta[ii]-v[0]*C[ii][0])/h- (1-epsi)/epsi*rho_s*dqdt[ii][0]
+                dCdt_tmp[-1]= +(v[-2]*C[ii][-2]- v_out*C[ii][-1])/h - (1-epsi)/epsi*rho_s*dqdt[ii][-1]
+###################################################3
+#                dv0 = (v[0] - v_in)/h
+#                dC0 = (C[ii][0] - C_sta[ii])/h
+#
+#                dvL = (v_out-v[-2])/h
+#                dCL = (C[ii][-1] - C[ii][-2])/h
+#                dCdt_tmp[0] = -v[0]*dC0 - C[ii][0]*dv0 - (1-epsi)/epsi*rho_s*dqdt[ii][0]
+#                dCdt_tmp[-1]= -v_out*dCL-C[ii][-1]*dvL - (1-epsi)/epsi*rho_s*dqdt[ii][-1]
+###################################################3
+
                 dCdt.append(dCdt_tmp)
  
             dydt_tmp = dCdt+dqdt
             dydt = np.concatenate(dydt_tmp)
             return dydt
         
         C_init = []
@@ -410,16 +475,409 @@
         self._Tg_res = np.ones([len(self._t), 1])@np.reshape(self._Tg_init,[1,-1])
 
         if CPUtime_print:
             print('Simulation of this step is completed.')
             print('This took {0:9.3f} mins to run. \n'.format(toc))       
         return y_result, self._z, t_dom
 
-## Run mass & momentum & energy balance equations
+    def run_ma(self, t_max, n_sec = 5, CPUtime_print = False):
+        tic = time.time()/60
+        t_max_int = np.int32(np.floor(t_max), )
+        self._n_sec = n_sec
+        n_t = t_max_int*n_sec+ 1
+        n_comp = self._n_comp
+        D_dif = self._D_disp
+        C_sta = []
+        for ii in range(n_comp):
+            C_sta.append(self._y_in[ii]*self._P_in/R_gas/self._T_in*1E5)
+        Cbound = C_sta
+        k = np.array(self._k_mtc)*self._a_surf
+        T_const = self._T_in
+        P_ov = self._P_in
+        rho = self._rho_s
+        epsi = self._epsi
+        u0 = self._Q_in/epsi/self._A
+        N = self._N
+        
+        # Difference matrix
+        d = self._d
+        dd = self._dd
+
+        t_dom = np.linspace(0,t_max_int, n_t)
+        if t_max_int < t_max:
+            t_dom = np.concatenate((t_dom, [t_max]))
+        
+        def massonly(y,t):
+            C = []
+            q = []
+            dC = []
+            ddC = []
+            for ii in range(n_comp):
+                C.append(y[ii*N:(ii+1)*N])
+                q.append(y[n_comp*N + ii*N : n_comp*N + (ii+1)*N])
+            
+            q_sta = []
+            P_part = []
+            C_ov = np.zeros([N,])
+            for ii in range(n_comp):
+                dC.append(d@C[ii])
+                ddC.append(dd@C[ii])
+                C_ov = C_ov + C[ii]
+            yfrac = []
+            for ii in range(n_comp):
+                yfrac_tmp = C[ii]/C_ov
+                P_part_tmp = yfrac_tmp*P_ov
+                yfrac.append(yfrac_tmp)
+                P_part.append(yfrac_tmp*P_ov) # in bar
+            q_sta = self._iso(P_part ,T_const)
+            #print(q_sta)
+            dqdt = []
+            for ii in range(n_comp):
+                dqdt_tmp = k[ii]*(q_sta[ii] - q[ii])
+                dqdt.append(dqdt_tmp)
+
+            v = u0
+            dCdt = []
+            dydt_pr = []
+            for ii in range(n_comp):
+                dCdt_tmp = -v*dC[ii] + D_dif[ii]*ddC[ii] - (1-epsi)/epsi*rho*dqdt[ii]
+                dCdt_tmp[0] = (v*Cbound[ii] -v*C[ii][0])*d[2,2] - (1-epsi)/epsi*rho*dqdt[ii][0]
+                dCdt.append(dCdt_tmp)
+                dydt_pr.append(dCdt_tmp)
+            for ii in range(n_comp):
+                dydt_pr.append(dqdt[ii])
+            dydt = np.concatenate(dydt_pr)
+            return dydt
+        C_init = []
+        q_init = []
+        for ii in range(n_comp):
+            C_tmp = self._y_init[ii]*self._P_init*1E5/R_gas/self._Tg_init
+            C_init.append(C_tmp)
+            q_tmp = self._q_init[ii]
+            q_init.append(q_tmp)
+        tic = time.time()/60
+        if self._required['Flow direction'] == 'Backward':
+            for ii in range(n_comp):
+                C_init[ii] = self._A_flip@C_init[ii]
+                q_init[ii] = self._A_flip@q_init[ii]
+        y0_tmp = C_init + q_init
+        y0 = np.concatenate(y0_tmp)
+        
+        #RUN
+        y_result = odeint(massonly, y0, t_dom,)
+        
+        if self._required['Flow direction'] == 'Backward':
+            y_tmp = []
+            for ii in range(n_comp*2):
+                mat_tmp = y_result[:, ii*N : (ii+1)*N]
+                y_tmp.append(mat_tmp@self._A_flip)
+            y_flip = np.concatenate(y_tmp, axis = 1)
+            y_result = y_flip
+        self._y = y_result
+        self._t = t_dom
+        toc = time.time()/60 - tic
+        self._CPU_min = toc
+        self._Tg_res = np.ones([len(self._t), 1])@np.reshape(self._Tg_init,[1,-1])
+
+        if CPUtime_print:
+            print('Simulation of this step is completed.')
+            print('This took {0:9.3f} mins to run. \n'.format(toc))       
+        return y_result, self._z, t_dom
+
+
+    def run_ma_POD(self, t_max, n_sec = 5, N_basis = 20, U_basis = None, CPUtime_print = False):
+        tic = time.time()/60
+        if (type(None)==type(U_basis)):
+            if self.is_BASIS:
+                U_basis = self._U_basis
+            else:
+                print("Please use 'find_basis' first to find the basis!")
+                return None
+        elif (type(U_basis) == type(np.array([1,2,3,]))):
+            if len(U_basis) <= 2:
+                if self.is_BASIS:
+                    U_basis = self._U_basis
+                else:
+                    print("Please use 'find_basis' first to find the basis!")
+                    return None
+        U_cut = U_basis[:,:N_basis]
+        
+        tic = time.time()/60
+        t_max_int = np.int32(np.floor(t_max), )
+        self._n_sec = n_sec
+        n_t = t_max_int*n_sec+ 1
+        n_comp = self._n_comp
+        D_dif = self._D_disp
+        C_sta = []
+        for ii in range(n_comp):
+            C_sta.append(self._y_in[ii]*self._P_in/R_gas/self._T_in*1E5)
+        Cbound = C_sta
+
+        k = np.array(self._k_mtc)*self._a_surf
+        T_const = self._T_in
+        P_ov = self._P_in
+        rho = self._rho_s
+        epsi = self._epsi
+        u0 = self._Q_in/epsi/self._A
+        N = self._N
+        
+        # Difference matrix
+        d = self._d
+        dd = self._dd
+
+        t_dom = np.linspace(0,t_max_int, n_t)
+        if t_max_int < t_max:
+            t_dom = np.concatenate((t_dom, [t_max]))
+        
+        def massonly(aa,t):
+            y = U_cut@aa
+            C = []
+            q = []
+            dC = []
+            ddC = []
+            for ii in range(n_comp):
+                C.append(y[ii*N:(ii+1)*N])
+                q.append(y[n_comp*N + ii*N : n_comp*N + (ii+1)*N])
+            
+            q_sta = []
+            P_part = []
+            C_ov = np.zeros([N,])
+            for ii in range(n_comp):
+                dC.append(d@C[ii])
+                ddC.append(dd@C[ii])
+                C_ov = C_ov + C[ii]
+            yfrac = []
+            for ii in range(n_comp):
+                yfrac_tmp = C[ii]/C_ov
+                P_part_tmp = yfrac_tmp*P_ov
+                yfrac.append(yfrac_tmp)
+                P_part.append(yfrac_tmp*P_ov) # in bar
+            q_sta = self._iso(P_part ,T_const)
+            #print(q_sta)
+            dqdt = []
+            for ii in range(n_comp):
+                dqdt_tmp = k[ii]*(q_sta[ii] - q[ii])
+                dqdt.append(dqdt_tmp)
+
+            v = u0
+            dCdt = []
+            dydt_pr = []
+            for ii in range(n_comp):
+                dCdt_tmp = -v*dC[ii] + D_dif[ii]*ddC[ii] - (1-epsi)/epsi*rho*dqdt[ii]
+                dCdt_tmp[0] = (v*Cbound[ii] -v*C[ii][0])*d[2,2] - (1-epsi)/epsi*rho*dqdt[ii][0]
+                dCdt.append(dCdt_tmp)
+                dydt_pr.append(dCdt_tmp)
+            for ii in range(n_comp):
+                dydt_pr.append(dqdt[ii])
+            dydt = np.concatenate(dydt_pr)
+            daadt = U_cut.T@dydt
+            return daadt
+        
+        C_init = []
+        q_init = []
+        for ii in range(n_comp):
+            C_tmp = self._y_init[ii]*self._P_init*1E5/R_gas/self._Tg_init
+            C_init.append(C_tmp)
+            q_tmp = self._q_init[ii]
+            q_init.append(q_tmp)
+
+        tic = time.time()/60
+        if self._required['Flow direction'] == 'Backward':
+            for ii in range(n_comp):
+                C_init[ii] = self._A_flip@C_init[ii]
+                q_init[ii] = self._A_flip@q_init[ii]
+        y0_tmp = C_init + q_init
+        y0 = np.concatenate(y0_tmp)
+        aa0 = U_cut.T@y0
+
+        #RUN
+        aa_result = odeint(massonly, aa0, t_dom,)
+        y_result = aa_result@U_cut.T
+        
+        if self._required['Flow direction'] == 'Backward':
+            y_tmp = []
+            for ii in range(n_comp*2):
+                mat_tmp = y_result[:, ii*N : (ii+1)*N]
+                y_tmp.append(mat_tmp@self._A_flip)
+            y_flip = np.concatenate(y_tmp, axis = 1)
+            y_result = y_flip
+        self._y = y_result
+        self._t = t_dom
+        toc = time.time()/60 - tic
+        self._CPU_min = toc
+        self._Tg_res = np.ones([len(self._t), 1])@np.reshape(self._Tg_init,[1,-1])
+
+        if CPUtime_print:
+            print('Simulation of this step is completed.')
+            print('This took {0:9.3f} mins to run. \n'.format(toc))       
+        return y_result, self._z, t_dom
+
+
+
+## Run mass & momentum balance equations
+    def run_mamo_POD(self, t_max, n_sec = 5, N_basis = 20, U_basis = None, CPUtime_print = False):
+        tic = time.time()/60
+        if (type(None)==type(U_basis)):
+            if self.is_BASIS:
+                U_basis = self._U_basis
+            else:
+                print("Please use 'find_basis' first to find the basis!")
+                return None
+        elif (type(U_basis) == type(np.array([1,2,3,]))):
+            if len(U_basis) <= 2:
+                if self.is_BASIS:
+                    U_basis = self._U_basis
+                else:
+                    print("Please use 'find_basis' first to find the basis!")
+                    return None
+                
+        U_cut = U_basis[:, :N_basis]
+        t_max_int = np.int32(np.floor(t_max), )
+        self._n_sec = n_sec
+        n_t = t_max_int*n_sec+ 1
+        n_comp = self._n_comp
+        C_sta = []
+        for ii in range(n_comp):
+            C_sta.append(self._y_in[ii]*self._P_in/R_gas/self._T_in*1E5)
+        t_dom = np.linspace(0,t_max_int, n_t)
+        if t_max_int < t_max:
+            t_dom = np.concatenate((t_dom, [t_max]))
+        #print(C1_sta)
+
+        # other parmeters
+        epsi = self._epsi
+        rho_s = self._rho_s
+
+        N = self._N
+        def massmomebal(aa,t):
+            y = U_cut@aa
+            C = []
+            q = []
+            for ii in range(n_comp):
+                C.append(y[ii*N:(ii+1)*N])
+                q.append(y[n_comp*N + ii*N : n_comp*N + (ii+1)*N])
+ 
+            # Derivatives
+            dC = []
+            ddC = []
+            C_ov = np.zeros(N)
+            P_ov = np.zeros(N)
+            P_part = []
+            Mu = np.zeros(N)
+            T = self._Tg_init
+            for ii in range(n_comp):
+                dC.append(self._d@C[ii])
+                ddC.append(self._dd@C[ii])
+                P_part.append(C[ii]*R_gas*T/1E5) # in bar
+                C_ov = C_ov + C[ii]
+                P_ov = P_ov + C[ii]*R_gas*T
+                Mu = Mu + C[ii]*self._mu[ii]
+            Mu = Mu/C_ov
+            #Mu = np.mean(self._mu)*np.ones_like(self._N)
+            # Ergun equation
+            v,dv = Ergun(C,T,self._M_m,Mu,self._D_p,epsi,
+                         self._d,self._dd,self._d_fo, self._N)
+            
+            # Solid phase
+            qsta = self._iso(P_part, T) # partial pressure in bar
+            dqdt = []
+            if self._order_MTC == 1:
+                for ii in range(n_comp):
+                    dqdt_tmp = self._k_mtc[ii]*(qsta[ii] - q[ii])*self._a_surf
+                    dqdt.append(dqdt_tmp)
+            elif self._order_MTC == 2:
+                for ii in range(n_comp):
+                    dqdt_tmp = self._k_mtc[ii][0]*(qsta[ii] - q[ii])*self._a_surf + self._k_mtc[ii][1]*(qsta[ii] - q[ii])**2*self._a_surf
+                    dqdt.append(dqdt_tmp)
+            # Valve equations (v_in and v_out)
+            #P_in = (C1_sta + C2_sta)*R_gas*T_gas
+            if self._const_v:
+                v_in = self._Q_in/epsi/self._A
+            else:
+                v_in = max(self._Cv_in*(self._P_in - P_ov[0]/1E5), 0 )  # pressure in bar           
+            v_out = max(self._Cv_out*(P_ov[-1]/1E5 - self._P_out), 0 )  # pressure in bar
+            
+            D_dis = self._D_disp
+            h = self._h
+            # Gas phase
+            dCdt = []
+            for ii in range(n_comp):
+                dCdt_tmp = -v*dC[ii] -C[ii]*dv + D_dis[ii]*ddC[ii] - (1-epsi)/epsi*rho_s*dqdt[ii]
+                #dCdt_tmp[0] = +(v_in*C_sta[ii] - v[1]*C[ii][0])/h - (1-epsi)/epsi*rho_s*dqdt[ii][0]
+                #dCdt_tmp[-1]= +(v[-1]*C[ii][-2]- v_out*C[ii][-1])/h - (1-epsi)/epsi*rho_s*dqdt[ii][-1]
+                #dCdt_tmp[0] = v_in*(C_sta[ii]-C[ii][0])/h- (1-epsi)/epsi*rho_s*dqdt[ii][0]
+                #dCdt_tmp[-1]= +(v_out+v[-1])/2*(C[ii][-2]- C[ii][-1])/h - (1-epsi)/epsi*rho_s*dqdt[ii][-1]
+                dCdt_tmp[0] = (v_in*C_sta[ii]-v[0]*C[ii][0])/h- (1-epsi)/epsi*rho_s*dqdt[ii][0]
+                dCdt_tmp[-1]= +(v[-2]*C[ii][-2]- v_out*C[ii][-1])/h - (1-epsi)/epsi*rho_s*dqdt[ii][-1]
+###################################################3
+#                dv0 = (v[0] - v_in)/h
+#                dC0 = (C[ii][0] - C_sta[ii])/h
+#
+#                dvL = (v_out-v[-2])/h
+#                dCL = (C[ii][-1] - C[ii][-2])/h
+#                dCdt_tmp[0] = -v[0]*dC0 - C[ii][0]*dv0 - (1-epsi)/epsi*rho_s*dqdt[ii][0]
+#                dCdt_tmp[-1]= -v_out*dCL-C[ii][-1]*dvL - (1-epsi)/epsi*rho_s*dqdt[ii][-1]
+###################################################3
+
+                dCdt.append(dCdt_tmp)
+ 
+            dydt_tmp = dCdt+dqdt
+            dydt = np.concatenate(dydt_tmp)
+            daadt = U_cut.T@dydt
+            return daadt
+        
+        C_init = []
+        q_init = []
+        for ii in range(n_comp):
+            C_tmp = self._y_init[ii]*self._P_init*1E5/R_gas/self._Tg_init
+            C_init.append(C_tmp)
+            q_tmp = self._q_init[ii]
+            q_init.append(q_tmp)
+ 
+        tic = time.time()/60
+        if self._required['Flow direction'] == 'Backward':
+            for ii in range(n_comp):
+                C_init[ii] = self._A_flip@C_init[ii]
+                q_init[ii] = self._A_flip@q_init[ii]
+        
+        y0_tmp = C_init + q_init
+        y0 = np.concatenate(y0_tmp)
+        
+        # Change the basis (coordinate)
+        aa0 = U_cut.T@y0
+
+        #RUN
+        aa_result = odeint(massmomebal,aa0,t_dom,)
+        
+        # Rolling back to Original coordinate
+        y_result = aa_result@U_cut.T
 
+        if self._required['Flow direction'] == 'Backward':
+            y_tmp = []
+            for ii in range(n_comp*2):
+                mat_tmp = y_result[:, ii*N : (ii+1)*N]
+                y_tmp.append(mat_tmp@self._A_flip)
+            y_flip = np.concatenate(y_tmp, axis = 1)
+            y_result = y_flip
+        self._y = y_result
+        self._t = t_dom
+        toc = time.time()/60 - tic
+        self._CPU_min = toc
+        self._Tg_res = np.ones([len(self._t), 1])@np.reshape(self._Tg_init,[1,-1])
+
+        if CPUtime_print:
+            print('Simulation of this step is completed.')
+            print('This took {0:9.3f} mins to run. \n'.format(toc))       
+        return y_result, self._z, t_dom
+
+
+
+
+
+## Run mass & momentum & energy balance equations
     def run_mamoen_alt(self, t_max, n_sec = 5, CPUtime_print = False):
         t_max_int = np.int32(np.floor(t_max))
         self._n_sec = n_sec
         n_t = t_max_int*n_sec+ 1
         n_comp = self._n_comp
         
         t_dom = np.linspace(0,t_max_int, n_t)
@@ -481,15 +939,15 @@
             # Viscosity
             for ii in range(n_comp):
                 dC.append(self._d@C[ii])
                 ddC.append(self._dd@C[ii])
                 P_part.append(C[ii]*R_gas*Tg/1E5) # in bar
                 C_ov = C_ov + C[ii]
                 P_ov = P_ov + C[ii]*R_gas*Tg
-                Mu = C[ii]*self._mu[ii]
+                Mu = Mu + C[ii]*self._mu[ii]
             Mu = Mu/C_ov
 
             # Ergun equation
             v,dv = Ergun(C,Tg,self._M_m,Mu,self._D_p,epsi,
                          self._d,self._dd,self._d_fo, self._N)
             
             # Solid phase concentration
@@ -512,16 +970,18 @@
             v_out = max(self._Cv_out*(P_ov[-1]/1E5 - self._P_out), 0 )  # pressure in bar
             
             # Gas phase concentration
             dCdt = []
             for ii in range(n_comp):
                 dCdt_tmp = -v*dC[ii] -C[ii]*dv + D_dis[ii]*ddC[ii] - (1-epsi)/epsi*rho_s*dqdt[ii]
                 #dCdt_tmp[0] = +(v_in*C_sta[ii] - v[1]*C[ii][0])/h - (1-epsi)/epsi*rho_s*dqdt[ii][0]    
-                dCdt_tmp[0] = +v_in*(C_sta[ii] - C[ii][0])/h - (1-epsi)/epsi*rho_s*dqdt[ii][0]
-                dCdt_tmp[-1]= +(v_out+v[-1])/2*(C[ii][-2]- C[ii][-1])/h - (1-epsi)/epsi*rho_s*dqdt[ii][-1]
+                #dCdt_tmp[0] = +v_in*(C_sta[ii] - C[ii][0])/h - (1-epsi)/epsi*rho_s*dqdt[ii][0]
+                #dCdt_tmp[-1]= +(v_out+v[-1])/2*(C[ii][-2]- C[ii][-1])/h - (1-epsi)/epsi*rho_s*dqdt[ii][-1]
+                dCdt_tmp[0] = (v_in*C_sta[ii]-v[0]*C[ii][0])/h- (1-epsi)/epsi*rho_s*dqdt[ii][0]
+                dCdt_tmp[-1]= +(v[-2]*C[ii][-2]- v_out*C[ii][-1])/h - (1-epsi)/epsi*rho_s*dqdt[ii][-1]
                 dCdt.append(dCdt_tmp)
             # Temperature (gas)
             Cov_Cpg = np.zeros(N) # Heat capacity (overall) J/K/m^3
             for ii in range(n_comp):
                 Cov_Cpg = Cov_Cpg + Cpg[ii]*C[ii]
             dTgdt = -v*dTg + h_heat*a_surf/epsi*(Ts - Tg)/Cov_Cpg
             for ii in range(n_comp):
@@ -619,15 +1079,15 @@
 
         C_sta = []
         Cov_Cpg_in = 0
         for ii in range(n_comp):
             C_sta.append(self._y_in[ii]*self._P_in/R_gas/self._T_in*1E5)
             Cov_Cpg_in = Cov_Cpg_in + Cpg[ii]*C_sta[ii]
         
-        def massmomeenerbal(y,t):
+        def massmomeenerbal(y, t):
             C = []
             q = []
             for ii in range(n_comp):
                 C.append(y[ii*N:(ii+1)*N])
                 q.append(y[n_comp*N + ii*N : n_comp*N + (ii+1)*N])
             Tg = y[2*n_comp*N : 2*n_comp*N + N ]
             Ts = y[2*n_comp*N + N : 2*n_comp*N + 2*N ]
@@ -650,16 +1110,17 @@
             # Viscosity
             for ii in range(n_comp):
                 dC.append(self._d@C[ii])
                 ddC.append(self._dd@C[ii])
                 P_part.append(C[ii]*R_gas*Tg/1E5) # in bar
                 C_ov = C_ov + C[ii]
                 P_ov = P_ov + C[ii]*R_gas*Tg
-                Mu = C[ii]*self._mu[ii]
+                Mu = Mu + C[ii]*self._mu[ii]
             Mu = Mu/C_ov
+             
 
             # Ergun equation
             v,dv = Ergun(C,Tg,self._M_m,Mu,self._D_p,epsi,
                          self._d,self._dd,self._d_fo, self._N)
             
             # Solid phase concentration
             qsta = self._iso(P_part, Tg) # partial pressure in bar
@@ -674,39 +1135,51 @@
                     dqdt.append(dqdt_tmp)
             # Valve equations (v_in and v_out)
             #P_in = (C1_sta + C2_sta)*R_gas*T_gas
             if self._const_v:
                 v_in = self._Q_in/epsi/self._A
             else:
                 v_in = max(self._Cv_in*(self._P_in - P_ov[0]/1E5), 0 )  # pressure in bar           
+                v_in = self._Cv_in*(self._P_in - P_ov[0]/1E5)  # pressure in bar           
             v_out = max(self._Cv_out*(P_ov[-1]/1E5 - self._P_out), 0 )  # pressure in bar
             
             # Gas phase concentration
             dCdt = []
             for ii in range(n_comp):
                 dCdt_tmp = -v*dC[ii] -C[ii]*dv + D_dis[ii]*ddC[ii] - (1-epsi)/epsi*rho_s*dqdt[ii]
-                dCdt_tmp[0] = +(v_in*C_sta[ii] - v[1]*C[ii][0])/h - (1-epsi)/epsi*rho_s*dqdt[ii][0]    
+                #dCdt_tmp[0] = +(v_in*C_sta[ii] - v[1]*C[ii][0])/h - (1-epsi)/epsi*rho_s*dqdt[ii][0]    
                 #dCdt_tmp[0] = +(v_in*C_sta[ii] - v[1]*C[ii][0])/h - (1-epsi)/epsi*rho_s*dqdt[ii][0]
-                dCdt_tmp[-1]= +(v[-1]*C[ii][-2]- v_out*C[ii][-1])/h - (1-epsi)/epsi*rho_s*dqdt[ii][-1]
+                #dCdt_tmp[-1]= +(v[-1]*C[ii][-2]- v_out*C[ii][-1])/h - (1-epsi)/epsi*rho_s*dqdt[ii][-1]
+                dCdt_tmp[0] = (v_in*C_sta[ii]-v[0]*C[ii][0])/h- (1-epsi)/epsi*rho_s*dqdt[ii][0]
+                dCdt_tmp[-1]= +(v[-2]*C[ii][-2]- v_out*C[ii][-1])/h - (1-epsi)/epsi*rho_s*dqdt[ii][-1]
+###################################################3
+                dv0 = (v[0] - v_in)/h
+                dC0 = (C[ii][0] - C_sta[ii])/h
+
+                dvL = (v_out-v[-2])/h
+                dCL = (C[ii][-1] - C[ii][-2])/h
+                dCdt_tmp[0] = -v[0]*dC0 - C[ii][0]*dv0 - (1-epsi)/epsi*rho_s*dqdt[ii][0]
+                dCdt_tmp[-1]= -v_out*dCL-C[ii][-1]*dvL - (1-epsi)/epsi*rho_s*dqdt[ii][-1]
+###################################################3
                 dCdt.append(dCdt_tmp)
             # Temperature (gas)
             Cov_Cpg = np.zeros(N) # Heat capacity (overall) J/K/m^3
             for ii in range(n_comp):
                 Cov_Cpg = Cov_Cpg + Cpg[ii]*C[ii]
             dTgdt = -v*dTg + h_heat*a_surf/epsi*(Ts - Tg)/Cov_Cpg
             for ii in range(n_comp):
                 dTgdt = dTgdt - Cpg[ii]*Tg*D_dis[ii]*ddC[ii]/Cov_Cpg
                 dTgdt = dTgdt + Tg*self._rho_s*(1-epsi)/epsi*Cpg[ii]*dqdt[ii]/Cov_Cpg
                 dTgdt = dTgdt + h_ambi*4/epsi/D_col*(T_ambi - Tg)/Cov_Cpg
 
             dTgdt[0] = h_heat*a_surf/epsi*(Ts[0] - Tg[0])/Cov_Cpg[0]
-            dTgdt[0] = dTgdt[0] + (v_in*self._T_in*Cov_Cpg_in/Cov_Cpg[0] - v[1]*Tg[0])/h
+            dTgdt[0] = dTgdt[0] + (v_in*self._T_in*Cov_Cpg_in/Cov_Cpg[0] - v[0]*Tg[0])/h
             dTgdt[-1] = h_heat*a_surf/epsi*(Ts[-1] - Tg[-1])/Cov_Cpg[-1]
             #dTgdt[-1] = dTgdt[-1] + (v[-1]*Tg[-2]*Cov_Cpg[-2]/Cov_Cpg[-1] - v_out*Tg[-1])/h
-            dTgdt[-1] = dTgdt[-1] + (v[-1]*Tg[-2]*Cov_Cpg[-2]/Cov_Cpg[-1] - v_out*Tg[-1])/h
+            dTgdt[-1] = dTgdt[-1] + (v[-2]*Tg[-2]*Cov_Cpg[-2]/Cov_Cpg[-1] - v_out*Tg[-1])/h
             for ii in range(n_comp):
                 dTgdt[0] = dTgdt[0] - Tg[0]*Cpg[ii]*dCdt[ii][0]/Cov_Cpg[0]
                 dTgdt[-1] = dTgdt[-1] - Tg[-1]*Cpg[ii]*dCdt[ii][-1]/Cov_Cpg[-1]
             dTsdt = (self._k_cond*ddTs+ h_heat*a_surf/(1-epsi)*(Tg-Ts))/self._rho_s/Cps
             for ii in range(n_comp):
                 dTsdt = dTsdt + abs(dH[ii])*dqdt[ii]/Cps
             
@@ -729,28 +1202,270 @@
                 q_init[ii] = self._A_flip@q_init[ii]
             y0_tmp = C_init + q_init + [self._A_flip@self._Tg_init] + [self._A_flip@self._Ts_init]
         else:
             y0_tmp = C_init + q_init + [self._Tg_init] + [self._Ts_init]
         y0 = np.concatenate(y0_tmp)
         
         #RUN
-        y_result = odeint(massmomeenerbal,y0,t_dom,)
+        y_result = odeint(massmomeenerbal,y0, t_dom,)
+        #y_ivp = solve_ivp(massmomeenerbal,t_dom, y0,method = 'BDF')
+        #y_result = y_ivp.y
         C_sum = 0
         for ii in range(n_comp):
             C_sum = C_sum + y_result[-1,ii*N+2]
         if C_sum  < 0.1:
             y_result, _,_  = self.run_mamoen_alt(t_max,n_sec)
             toc = time.time()/60 - tic
             self._CPU_min = toc
             self._Tg_res = y_result[:,n_comp*2*N : n_comp*2*N+N]
             if CPUtime_print:
                 print('Simulation of this step is completed.')
                 print('This took {0:9.3f} mins to run. \n'.format(toc))
-            return y_result
+            return y_result, self._z, t_dom
+        
+        if self._required['Flow direction'] == 'Backward':
+            y_tmp = []
+            for ii in range(n_comp*2 + 2):
+                mat_tmp = y_result[:, ii*N : (ii+1)*N]
+                y_tmp.append(mat_tmp@self._A_flip)
+            y_flip = np.concatenate(y_tmp, axis = 1)
+            y_result = y_flip
+        self._y = y_result
+        self._t = t_dom
+        toc = time.time()/60 - tic
+        self._CPU_min = toc
+        self._Tg_res = y_result[:,n_comp*2*N : n_comp*2*N+N]
+        if CPUtime_print:
+            print('Simulation of this step is completed.')
+            print('This took {0:9.3f} mins to run. \n'.format(toc))       
+        return y_result, self._z, t_dom
+
+    def find_basis(self, show_graph = False, show_n = 20):
+        try:
+            self._y
+        except:
+            print("You have to run the simulation, first!")
+            return
+        U, Sig, Vt = np.linalg.svd(self._y.T)
+        self.is_BASIS = True
+        self._U_basis = U
+        if show_graph:
+            if show_n == -1:
+                fig = plt.figure()
+                plt.bar(np.arange(1,len(U)), 
+                         Sig,
+                         color = 'k')
+                plt.xlabel("Principle components")
+                plt.ylabel("Singular value")
+            else:
+                fig = plt.figure()
+                plt.bar(np.arange(1,show_n+1), 
+                        Sig[:show_n],
+                        color = 'k')
+                plt.xlabel("Principle components")
+                plt.ylabel("Singular value")
+            return U, Sig, Vt, fig
+        
+        return U, Sig, Vt
+        
+
+    def run_mamoen_POD(self, t_max, n_sec = 5, N_basis = 20, U_basis = None, CPUtime_print = False):
+        if (type(None)==type(U_basis)):
+            if self.is_BASIS:
+                U_basis = self._U_basis
+            else:
+                print("Please use 'find_basis' first to find the basis!")
+                return None
+        elif (type(U_basis) == type(np.array([1,2,3,]))):
+            if len(U_basis) <= 2:
+                if self.is_BASIS:
+                    U_basis = self._U_basis
+                else:
+                    print("Please use 'find_basis' first to find the basis!")
+                    return None
+        U_cut = U_basis[:,:N_basis]
+        t_max_int = np.int32(np.floor(t_max))
+        self._n_sec = n_sec
+        n_t = t_max_int*n_sec+ 1
+        n_comp = self._n_comp
+        
+        t_dom = np.linspace(0,t_max_int, n_t)
+        if t_max_int < t_max:
+            t_dom = np.concatenate((t_dom, [t_max]))
+        
+        N = self._N
+        h = self._h
+        epsi = self._epsi
+        a_surf = self._a_surf
+
+        # Mass
+        D_dis = self._D_disp
+        k_mass = self._k_mtc
+
+        # Heat
+        dH = self._dH
+        Cpg = self._Cp_g
+        Cps = self._Cp_s
+
+        h_heat = self._h_heat
+        h_ambi = self._h_ambi
+        T_ambi = self._T_ambi
+
+        # other parmeters
+        rho_s = self._rho_s
+        D_col = np.sqrt(self._A/np.pi)*2
+
+        C_sta = []
+        Cov_Cpg_in = 0
+        for ii in range(n_comp):
+            C_sta.append(self._y_in[ii]*self._P_in/R_gas/self._T_in*1E5)
+            Cov_Cpg_in = Cov_Cpg_in + Cpg[ii]*C_sta[ii]
         
+        def massmomeenerbal(aa, t):
+            y = U_cut@aa
+            C = []
+            q = []
+            for ii in range(n_comp):
+                C.append(y[ii*N:(ii+1)*N])
+                q.append(y[n_comp*N + ii*N : n_comp*N + (ii+1)*N])
+            Tg = y[2*n_comp*N : 2*n_comp*N + N ]
+            Ts = y[2*n_comp*N + N : 2*n_comp*N + 2*N ]
+ 
+            # Derivatives
+            dC = []
+            ddC = []
+            C_ov = np.zeros(N)
+            P_ov = np.zeros(N)
+            P_part = []
+            Mu = np.zeros(N)
+            #T = self._Tg_init
+            # Temperature gradient:
+            dTg = self._d@Tg
+            ddTs = self._dd@Ts
+
+            # Concentration gradient
+            # Pressure (overall&partial)
+            # Viscosity
+            for ii in range(n_comp):
+                dC.append(self._d@C[ii])
+                ddC.append(self._dd@C[ii])
+                P_part.append(C[ii]*R_gas*Tg/1E5) # in bar
+                C_ov = C_ov + C[ii]
+                P_ov = P_ov + C[ii]*R_gas*Tg
+                Mu = Mu + C[ii]*self._mu[ii]
+            Mu = Mu/C_ov
+             
+
+            # Ergun equation
+            v,dv = Ergun(C,Tg,self._M_m,Mu,self._D_p,epsi,
+                         self._d,self._dd,self._d_fo, self._N)
+            
+            # Solid phase concentration
+            qsta = self._iso(P_part, Tg) # partial pressure in bar
+            dqdt = []
+            if self._order_MTC == 1:
+                for ii in range(n_comp):
+                    dqdt_tmp = self._k_mtc[ii]*(qsta[ii] - q[ii])*self._a_surf
+                    dqdt.append(dqdt_tmp)
+            elif self._order_MTC == 2:
+                for ii in range(n_comp):
+                    dqdt_tmp = self._k_mtc[ii][0]*(qsta[ii] - q[ii])*self._a_surf + self._k_mtc[ii][1]*(qsta[ii] - q[ii])**2*self._a_surf
+                    dqdt.append(dqdt_tmp)
+            # Valve equations (v_in and v_out)
+            #P_in = (C1_sta + C2_sta)*R_gas*T_gas
+            if self._const_v:
+                v_in = self._Q_in/epsi/self._A
+            else:
+                v_in = max(self._Cv_in*(self._P_in - P_ov[0]/1E5), 0 )  # pressure in bar           
+                v_in = self._Cv_in*(self._P_in - P_ov[0]/1E5)  # pressure in bar           
+            v_out = max(self._Cv_out*(P_ov[-1]/1E5 - self._P_out), 0 )  # pressure in bar
+            
+            # Gas phase concentration
+            dCdt = []
+            for ii in range(n_comp):
+                dCdt_tmp = -v*dC[ii] -C[ii]*dv + D_dis[ii]*ddC[ii] - (1-epsi)/epsi*rho_s*dqdt[ii]
+                #dCdt_tmp[0] = +(v_in*C_sta[ii] - v[1]*C[ii][0])/h - (1-epsi)/epsi*rho_s*dqdt[ii][0]    
+                #dCdt_tmp[0] = +(v_in*C_sta[ii] - v[1]*C[ii][0])/h - (1-epsi)/epsi*rho_s*dqdt[ii][0]
+                #dCdt_tmp[-1]= +(v[-1]*C[ii][-2]- v_out*C[ii][-1])/h - (1-epsi)/epsi*rho_s*dqdt[ii][-1]
+                dCdt_tmp[0] = (v_in*C_sta[ii]-v[0]*C[ii][0])/h- (1-epsi)/epsi*rho_s*dqdt[ii][0]
+                dCdt_tmp[-1]= +(v[-2]*C[ii][-2]- v_out*C[ii][-1])/h - (1-epsi)/epsi*rho_s*dqdt[ii][-1]
+###################################################3
+                dv0 = (v[0] - v_in)/h
+                dC0 = (C[ii][0] - C_sta[ii])/h
+
+                dvL = (v_out-v[-2])/h
+                dCL = (C[ii][-1] - C[ii][-2])/h
+                dCdt_tmp[0] = -v[0]*dC0 - C[ii][0]*dv0 - (1-epsi)/epsi*rho_s*dqdt[ii][0]
+                dCdt_tmp[-1]= -v_out*dCL-C[ii][-1]*dvL - (1-epsi)/epsi*rho_s*dqdt[ii][-1]
+###################################################3
+                dCdt.append(dCdt_tmp)
+            # Temperature (gas)
+            Cov_Cpg = np.zeros(N) # Heat capacity (overall) J/K/m^3
+            for ii in range(n_comp):
+                Cov_Cpg = Cov_Cpg + Cpg[ii]*C[ii]
+            dTgdt = -v*dTg + h_heat*a_surf/epsi*(Ts - Tg)/Cov_Cpg
+            for ii in range(n_comp):
+                dTgdt = dTgdt - Cpg[ii]*Tg*D_dis[ii]*ddC[ii]/Cov_Cpg
+                dTgdt = dTgdt + Tg*self._rho_s*(1-epsi)/epsi*Cpg[ii]*dqdt[ii]/Cov_Cpg
+                dTgdt = dTgdt + h_ambi*4/epsi/D_col*(T_ambi - Tg)/Cov_Cpg
+
+            dTgdt[0] = h_heat*a_surf/epsi*(Ts[0] - Tg[0])/Cov_Cpg[0]
+            dTgdt[0] = dTgdt[0] + (v_in*self._T_in*Cov_Cpg_in/Cov_Cpg[0] - v[0]*Tg[0])/h
+            dTgdt[-1] = h_heat*a_surf/epsi*(Ts[-1] - Tg[-1])/Cov_Cpg[-1]
+            #dTgdt[-1] = dTgdt[-1] + (v[-1]*Tg[-2]*Cov_Cpg[-2]/Cov_Cpg[-1] - v_out*Tg[-1])/h
+            dTgdt[-1] = dTgdt[-1] + (v[-2]*Tg[-2]*Cov_Cpg[-2]/Cov_Cpg[-1] - v_out*Tg[-1])/h
+            for ii in range(n_comp):
+                dTgdt[0] = dTgdt[0] - Tg[0]*Cpg[ii]*dCdt[ii][0]/Cov_Cpg[0]
+                dTgdt[-1] = dTgdt[-1] - Tg[-1]*Cpg[ii]*dCdt[ii][-1]/Cov_Cpg[-1]
+            dTsdt = (self._k_cond*ddTs+ h_heat*a_surf/(1-epsi)*(Tg-Ts))/self._rho_s/Cps
+            for ii in range(n_comp):
+                dTsdt = dTsdt + abs(dH[ii])*dqdt[ii]/Cps
+            
+            dydt_tmp = dCdt+dqdt+[dTgdt] + [dTsdt]
+            dydt = np.concatenate(dydt_tmp)
+            daadt = U_cut.T@dydt
+            return daadt
+        
+        C_init = []
+        q_init = []
+        for ii in range(n_comp):
+            C_tmp = self._y_init[ii]*self._P_init*1E5/R_gas/self._Tg_init
+            C_init.append(C_tmp)
+            q_tmp = self._q_init[ii]
+            q_init.append(q_tmp)
+ 
+        tic = time.time()/60
+        if self._required['Flow direction'] == 'Backward':
+            for ii in range(n_comp):
+                C_init[ii] = self._A_flip@C_init[ii]
+                q_init[ii] = self._A_flip@q_init[ii]
+            y0_tmp = C_init + q_init + [self._A_flip@self._Tg_init] + [self._A_flip@self._Ts_init]
+        else:
+            y0_tmp = C_init + q_init + [self._Tg_init] + [self._Ts_init]
+        y0 = np.concatenate(y0_tmp)
+        aa0 = U_cut.T@y0
+        #RUN
+        a_result = odeint(massmomeenerbal, aa0, t_dom,)
+        y_result = a_result@U_cut.T
+        #y_ivp = solve_ivp(massmomeenerbal,t_dom, y0,method = 'BDF')
+        #y_result = y_ivp.y
+        C_sum = 0
+        '''
+        for ii in range(n_comp):
+            C_sum = C_sum + y_result[-1,ii*N+2]
+        if C_sum  < 0.1:
+            y_result, _,_  = self.run_mamoen_alt(t_max,n_sec)
+            toc = time.time()/60 - tic
+            self._CPU_min = toc
+            self._Tg_res = y_result[:,n_comp*2*N : n_comp*2*N+N]
+            if CPUtime_print:
+                print('Simulation of this step is completed.')
+                print('This took {0:9.3f} mins to run. \n'.format(toc))
+            return y_result, self._z, t_dom
+        '''
         if self._required['Flow direction'] == 'Backward':
             y_tmp = []
             for ii in range(n_comp*2 + 2):
                 mat_tmp = y_result[:, ii*N : (ii+1)*N]
                 y_tmp.append(mat_tmp@self._A_flip)
             y_flip = np.concatenate(y_tmp, axis = 1)
             y_result = y_flip
@@ -1068,15 +1783,15 @@
     n_t = t_max_int*n_sec+ 1
     n_comp = column1._n_comp
     
     # Target pressure
     C_sta1 = np.zeros(n_comp)
     for ii in range(n_comp):
         C_sta1[ii] = c1_tmp._y_init[ii][0]*P_mean/R_gas/T_mean*1E5
-    print(C_sta1)
+    #print(C_sta1)
 
     t_dom = np.linspace(0,t_max_int, n_t)
     column1._n_sec = n_sec
     column2._n_sec = n_sec
     if t_max_int < t_max:
         t_dom = np.concatenate((t_dom, [t_max]))
 
@@ -2159,25 +2874,25 @@
         numor0 = isopar1[0]*b1*P[0]
         numor1 = isopar2[0]*b2*P[1]
         q_return = [numor0/denom, numor1/denom]
         return q_return
  
     epsi_test = 0.4         # macroscopic void fraction (m^3/m^3)
     D_particle_dia = 0.01   # particle diameter (m)
-    rho_s_test = 1100       # solid density (kg/mol)
+    rho_s_test = 1100       # solid density (kg/m^3)
     c1.adsorbent_info(iso_fn_test,epsi_test,D_particle_dia, rho_s_test)
  
     M_m_test  = [0.044, 0.028]      ## molar mass    (kg/mol)
     mu_test = [1.47E-5, 1.74E-5]    ## gas viscosity (Pa sec)
     c1.gas_prop_info(M_m_test, mu_test)
  
     ## Mass transfer coefficients
     D_dis_test = [1E-6, 1E-6]   # m^2/sec
     k_MTC = [0.0002, 0.0002]    # m/sec
-    a_surf = 400                # m^2/m^3
+    a_surf = 200                # m^2/m^3
     c1.mass_trans_info(k_MTC, a_surf, D_dis_test)
 
     ## Thermal properties
     Del_H = [30E3, 20E3]    # J/mol
     Cp_s = 935              # J/kg/K
     Cp_g = [37.22, 29.15]   # J/mol/K
     h_heat = 100            # J/sec/m^2/K
@@ -2218,25 +2933,26 @@
     c2 = c1.copy()
     c1.next_init()
 
     c1.boundaryC_info(Pout_test,Pin_test,Tin_test,yin_test,
     0.0*Cvin_test,Cvout_test,Q_in_test,False, foward_flow_direction=True)
     c2.boundaryC_info(Pout_test,Pin_test,Tin_test,yin_test,
     0.0*Cvin_test,0,Q_in_test,False, foward_flow_direction=True)
-
+    '''
     step_P_eq(
         c1,c2,100,n_sec = 50,
         valve_select = [1,1],
         Cv_btw=0.05,CPUtime_print=True)
     plt.show()
     Legend_loc = [1.15, 0.9]
     c1.Graph_P(10, loc = Legend_loc)
     c1.Graph(10,2, loc =Legend_loc)
     c1.Graph(10,3, loc =Legend_loc)
     c2.Graph_P(10, loc =Legend_loc)
     c2.Graph(10,2, loc =Legend_loc)
     c2.Graph(10,3, loc = Legend_loc)
     plt.show( )
+    '''
     
 # %%
 
 # %%
```

### Comparing `pyapep-0.1.0/setup.py` & `pyapep-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
         name='pyapep',
-        version='0.1.0',
+        version='0.1.2',
         author_email='sgasga@ulsan.ac.kr',
         description='Python package for adsorption process simulations',
         long_description_content_type='text/markdown',
         url='https://nahyeonan.github.io/pyAPEP/build/html/index.html',
         packages=setuptools.find_packages(),
         classifieres=[
             'Programming Language :: Python :: 3',
```

