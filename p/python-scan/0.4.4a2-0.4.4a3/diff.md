# Comparing `tmp/python_scan-0.4.4a2-py3-none-any.whl.zip` & `tmp/python_scan-0.4.4a3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 12959 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat    42776 b- defN 23-May-05 20:03 python_scan-0.4.4a2.data/scripts/PORT_SCAN.py
--rw-rw-rw-  2.0 fat     2777 b- defN 23-May-06 09:06 python_scan-0.4.4a2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-06 09:06 python_scan-0.4.4a2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        1 b- defN 23-May-06 09:06 python_scan-0.4.4a2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      424 b- defN 23-May-06 09:06 python_scan-0.4.4a2.dist-info/RECORD
-5 files, 46070 bytes uncompressed, 12163 bytes compressed:  73.6%
+Zip file size: 13609 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat    45497 b- defN 23-May-14 12:25 python_scan-0.4.4a3.data/scripts/PORT_SCAN.py
+-rw-rw-rw-  2.0 fat     3129 b- defN 23-May-14 12:25 python_scan-0.4.4a3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-14 12:25 python_scan-0.4.4a3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        1 b- defN 23-May-14 12:25 python_scan-0.4.4a3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      424 b- defN 23-May-14 12:25 python_scan-0.4.4a3.dist-info/RECORD
+5 files, 49143 bytes uncompressed, 12813 bytes compressed:  73.9%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
-Filename: python_scan-0.4.4a2.data/scripts/PORT_SCAN.py
+Filename: python_scan-0.4.4a3.data/scripts/PORT_SCAN.py
 Comment: 
 
-Filename: python_scan-0.4.4a2.dist-info/METADATA
+Filename: python_scan-0.4.4a3.dist-info/METADATA
 Comment: 
 
-Filename: python_scan-0.4.4a2.dist-info/WHEEL
+Filename: python_scan-0.4.4a3.dist-info/WHEEL
 Comment: 
 
-Filename: python_scan-0.4.4a2.dist-info/top_level.txt
+Filename: python_scan-0.4.4a3.dist-info/top_level.txt
 Comment: 
 
-Filename: python_scan-0.4.4a2.dist-info/RECORD
+Filename: python_scan-0.4.4a3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `python_scan-0.4.4a2.data/scripts/PORT_SCAN.py` & `python_scan-0.4.4a3.data/scripts/PORT_SCAN.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 
 except Exception as e:
     # If there are any errors encountered during the importing of the modules,
     # then we display the error message on the console screen
     print('Existen modulos necesarios que no tiene instalado... \n\n', e)
     exit()
 
-# Subir a pypi
 # añadir más opciones, como escaneo de webs (http-enum) / sqlinjection / brute force / etc...
 # Añadir Logs en el arhchivo (ip/puertos/vulns/etc...)
 
 if modules:
     nm = nmap.PortScanner()
     open_ports = []
 
@@ -137,17 +136,17 @@
         else:
             try:
                 ports = int(ports)
                 if ports > 65535:
                     input('Has superado el número máximo de puertos.\n'
                           'Se reducirá a "65535" (numero máx. de puertos) -- [ENTER]')
                     ports = 65535
-                    write_file('[!] PORTS TO SCAN ---> 1-' + str(ports))
+                    write_file(f'[!] PORTS TO SCAN ---> 1-{str(ports)}\n')
                 else:
-                    write_file('[!] PORTS TO SCAN ---> 1-' + str(ports))
+                    write_file(f'[!] PORTS TO SCAN ---> 1-{str(ports)}\n')
                 break
             except ValueError:
                 print(Fore.RED + "Arguemnto inválido.\nPara obtener ayuda escriba --> '--help'")
 
 
 
 def port_scan_banner():
@@ -163,15 +162,15 @@
 ░▒ ░       ░ ▒ ▒░   ░▒ ░ ▒░    ░       ░ ░▒  ░ ░  ░  ▒     ▒   ▒▒ ░░ ░░   ░ ▒░
 ░░       ░ ░ ░ ▒    ░░   ░   ░         ░  ░  ░  ░          ░   ▒      ░   ░ ░ 
              ░ ░     ░                       ░  ░ ░            ░  ░         ░ 
                                                 ░                                                                                                 
                                                 
        [INFO] Herramienta para analizar puertos de una dirección IP 
              ║                                                 ║                                                                                             
-             ║                    v0.4.4.a2                    ║
+             ║                    v0.4.4.a3                    ║
              ╚══════► Escriba --help para obtener ayuda ◄══════╝
                     \n\n""")
 
 
 def host_disc_bann():
     print(Fore.RED + '''\n
                                .    .        s              ....             .       .                                 _                                 
@@ -186,15 +185,15 @@
  888E  888E  "*888*P"   .888888P`    ^%888*        X88888888hx. ..!     888&  .888888P`   ?8888u../  "*888*P"     ^Y8888*""  '8888c. .+  ^"8888*"    
 m888N= 888>    'Y"      `   ^"F        'Y"        !   "*888888888"      R888" `   ^"F      "8888P'     'Y"          `Y"       "88888%       "Y"      
  `Y"   888                                               ^"***"`         ""                  "P'                                "YP'                 
       J88"                                                                                                                                           
       @%                                                                                                                                             
     :" 
                                 [INFO] Herramienta para analizar puertos de una dirección IP                                                                                             
-                                     ║                    v0.4.4.a2                    ║
+                                     ║                    v0.4.4.a3                    ║
                                      ╚══════► Escriba --help para obtener ayuda ◄══════╝
     
     \n''')
 
 
 def service_scan_bann():
     print(Fore.GREEN + """\n
@@ -206,34 +205,34 @@
  ▀▀▀▀  ▀▀▀ .▀  ▀. ▀  ▀▀▀·▀▀▀  ▀▀▀      ▀▀▀▀ ·▀▀▀  ▀  ▀ ▀▀ █▪                                                                                            
 \n""")
 
 
 def help_discover():
     print(Fore.YELLOW + """
             ╔════════════════════════════════════════════════╗
-            ║   --  Usabilidad 'HOST DISCOVER' v0.4.4.a2 --  ║        
+            ║   --  Usabilidad 'HOST DISCOVER' v0.4.4.a3 --  ║        
             ╚════════════════════════════════════════════════╝\n\n""" +
 
           Fore.BLUE + "[♦]" + Fore.YELLOW + " Enter IP --> IP OBETIVO\n" +
           Fore.CYAN + """
                 ║       
                 ╚════ EJEMPLO --> [♦] ENTER IP -> 192.168.1.0/24\n""" +
 
           Fore.CYAN + """ 
                 ║       
                 ╚═► """ + Fore.BLUE + "[♦] " + Fore.YELLOW + "REQUERIMIENTO --> " + Fore.YELLOW + 'Mascara en formato CIDR\n\n')
 
 
 def graph_host():
-    print(Fore.BLUE + "\t[!] " + Fore.GREEN + '↓ EJEMPLOS ↓ \n')
-    print(Fore.LIGHTRED_EX + "\t\t║")
-    print("\t\t║══════► 192.168.1.0/24")
-    print("\t\t║")
-    print("\t\t╚══════► --help")
-    print(Fore.BLUE + '\n\n\t[♦] ' + Fore.YELLOW + 'Enter IP Range')
+    print(Fore.BLUE + "\t\t[!] " + Fore.GREEN + '↓ EJEMPLOS ↓ \n')
+    print(Fore.LIGHTRED_EX + "\t\t \t║")
+    print("\t\t\t║══════► 192.168.1.0/24")
+    print("\t\t\t║")
+    print("\t\t\t╚══════► --help")
+    print(Fore.BLUE + '\n\n\t\t[♦] ' + Fore.YELLOW + 'Enter IP Range')
 
 
 def init_host():
     now = datetime.now()
     print(Fore.RED + "[!] " + Fore.YELLOW + "Escaneo de subred iniciado...\n")
     print(Fore.RED + "[T] " + Fore.YELLOW + "", now, "\n")
 
@@ -247,32 +246,32 @@
         clean()
         host_disc_bann()
 
         if err:
             graph_host()
             print(Fore.RED + "[!] Has introducido una máscara inválida...")
 
-            print("\t\t║")
-            target = input("\t\t╚═► " + Fore.RESET)
+            print("\t\t\t║")
+            target = input("\t\t\t╚═► " + Fore.RESET)
 
         else:
             # Printear ayuda la 1ª vez que se ejecute
             graph_host()
-            print("\t\t║")
-            target = input("\t\t╚═► " + Fore.RESET)
+            print("\t\t\t║")
+            target = input("\t\t\t╚═► " + Fore.RESET)
 
         # Printear ayuda
         if 'help' in target:
             clean()
             host_disc_bann()
             help_discover()
             graph_host()
 
-            print("\t\t║")
-            target = input("\t\t╚═► " + Fore.RESET)
+            print("\t\t\t║")
+            target = input("\t\t\t╚═► " + Fore.RESET)
 
         # Comprobar si está bien escrita la IP
         else:
             mask = re.findall("/([0-9]+)$", target)
             mask = "".join(mask)
 
             try:
@@ -334,27 +333,33 @@
             print_help()
 
             print(Fore.YELLOW + "\nQue herramienta quieres utilizar?")
             print("-" * 50)
             print(Fore.BLUE + 'A:' + Fore.YELLOW + ' --> Port and vuln scan' + '\n \n'
                   + Fore.BLUE + 'B:' + Fore.YELLOW + ' --> Metasploit.\n')
             fun = None
+
+        # Entramos en Port scan
         elif fun.lower() in ['a']:
             enter_arguments()
-            break
+            funcions()
 
+        # Entramos en metasploit
         elif fun.lower() in ['b']:
-            input(Fore.YELLOW + "Esta funcion requiere que tengas instalado Metasploit [-ENTER-].")
+            input(Fore.YELLOW + "[!] Esta funcion requiere que tengas instalado Metasploit [-ENTER-].")
             try:
                 os.system('msfconsole')
                 break
             except Exception as error:
-                print(Fore.RED + "ERROR: {}\nPrueba a reinstalar o instalar metasploit.".format(error))
+                print(Fore.RED + "[!] ERROR: {}\nPrueba a reinstalar o instalar metasploit.".format(error))
+
+        # Entramos en host discover
         elif fun.lower() in ['c']:
             host_discover()
+            funcions()
 
         else:
             print(Fore.RED + "Introduce una opción válida, has escogido '{}',"
                              " que no está entre las opciones disponibles".format(fun))
             fun = None
 
 
@@ -362,16 +367,16 @@
     global alive
     while True:
         clean()
         port_scan_banner()
         # Confirmación con PING?
 
         p = input(Fore.YELLOW + '[!] ¿Quieres hacer una confirmación con PING?\n\n' + Fore.GREEN
-                    + '\t[I] El host puede tener un FireWall bien configurado que bloquee este tipo de paquetes.\n'
-                    '\t     Si sabes que esta activo no ejecutes la confirmación.' + Fore.LIGHTRED_EX + '\n\t\t\t[S/n] -->')
+                                + '\t[I] El host puede tener un FireWall bien configurado que bloquee este tipo de paquetes.\n'
+            '\t   Si sabes que esta activo no ejecutes la confirmación.' + Fore.LIGHTRED_EX + '\n\n\t[S/n] --> ')
 
         # En línea o no
         if p in ['S', 's']:
 
             """
             Pings the given IP address to check if it's active or not.
             """
@@ -408,29 +413,30 @@
         # Si resulta victorioisa la conexion informamos de puerto abierto
         if result == 0:
             open_ports.append(port)
             clean()
             port_scan_banner()
             init(now, target)
             for open_port in open_ports:
-                print(Fore.BLUE + "[♦]" + Fore.YELLOW + " - El puerto {} esta abierto.".format(open_port), end="")
+                print(Fore.BLUE + "[♦]" + Fore.YELLOW + f" - El puerto {open_port} esta abierto.", end="")
                 print("\n" + "-" * 55 + "\n", end="")
         s.close()
 
     with concurrent.futures.ThreadPoolExecutor(max_workers=25) as executor:
         futures = []
         for port in range(1, ports + 1):
             try:
                 time.sleep(0.08)
                 futures.append(executor.submit(scaning, port))
             # Excepciones del código
             except KeyboardInterrupt:
                 end = datetime.now()
                 elapsed = end - now
                 print(Fore.YELLOW + '\n\nAnálisis interrumpido en el puerto {}.'.format(port))
+                write_file(f"\n[!] Port Scan interrupt in port {port} {elapsed}")
                 break
             except Exception as err:
                 print("Error inesperado : {}".format(err))
 
 
 def scan(target):
     try:
@@ -463,32 +469,37 @@
         print(Fore.RED + "\nNo se ha encontrado el HOST")
 
     now = datetime.now()
     init(now, target)
 
     init_scan(target, now)
 
-    # Final del analisis
+    # Final del analisis sin puertos
     end = datetime.now()
     if not open_ports:
         elapsed = end - now
         print(Fore.YELLOW + "\nTiempo transcurrido --> {}".format(elapsed))
         print(Fore.YELLOW + "\nNo se han detectado puertos abiertos. :_(")
+        write_file("[!] No open Ports exiting the program :'(")
         exit()
+
+    # Final del analisis con puertos encontrados
     print(Fore.YELLOW + "\nTiempo transcurrido --> {}".format((end - now)))
+    write_file("[*] END SCAN\n")
+    write_file(f"[*] ELAPSED --> {end - now}")
     ports_used(open_ports, target)
 
 
 def ports_used(open_ports, target):
     # Creamos lista ordenada de puertos para el scaner
     p_str = [str(a) for a in open_ports]
     p_str = (",".join(p_str))
     print(Fore.GREEN + "\n\nLos puertos abiertos son: {}".format(open_ports))
 
-    text = "[!] OPEN PORTS: {}".format(p_str)
+    text = "[!] OPEN PORTS: {}\n".format(p_str)
     write_file(text)
 
     # Iniciamos check services
     check_serv(target, p_str, open_ports)
 
 
 def serv_search():
@@ -612,29 +623,35 @@
         return default_args
     except Exception as err:
         print(err)
         time.sleep(2)
         return default_args
 
 
+def write_info_in_file():
+    pass
+
+
 def check_serv(target, p_str, open_ports):
     # Preguntamos si quiere analisis de versiones de servicio
     serv_search()
 
+    write_file('[!] Service Scan initiate\n')
+
     # Hora del inicio
     init_scan_service = datetime.now()
 
     # Argumentos de NMAP default
     default_args = "-p {} --script vuln -sS --min-rate 5000 -sC -sV -Pn --version-intensity 3 -n -A -O".format(p_str)
 
     args = know_nmap()
 
     # Comprobar los buenos comandos
     args = check_args(args, default_args, target, p_str)
-
+    write_file(f'[*] Nmap comman line {args}\n')
 
     # Inicio de análisis de nmap
     clean()
 
     # Inicio del escaneo
     graph_serv(init_scan_service)
     print(Fore.BLUE + "   [I] " + Fore.YELLOW + "Argumentos utilizados \n\t[{}]".format(args))
@@ -700,34 +717,65 @@
                     "[♦]" + Fore.YELLOW + " Nombre:" + Fore.GREEN + f"  {name}  |" +
                     Fore.YELLOW + "  Producto:" + Fore.GREEN + f" {product}   |" +
                     Fore.YELLOW + "  Versión:" + Fore.GREEN + f" {version}  |  {extrainfo}  |  " +
                     Fore.YELLOW + "CPE:" + Fore.GREEN + f" {cpe}  \n\nInfo: \n{script[0]}  \n")
 
                 print(Fore.GREEN + "\n" + "-" * 50, "\n")
 
+                text = f"""Puerto: {p}/{state} \n<--> Especificaciones del servicio <--> \n
+    [♦] Nombre: {name}    
+    Producto: {product}   
+    Versión: {version}  
+    Extra Info: {extrainfo}    
+    CPE: {cpe}  \n\n
+    Info: \n{script[0]}  \n""" + "\n" + "-" * 50 + "\n"
+
+                write_file(f"[!] FOUND INFORMATION ABOUT SERVICE!!\n")
+                write_file(text)
+
             else:
                 print(Fore.CYAN +
                       "Puerto: " + Fore.GREEN + f" {p}/{state} \n" + Fore.YELLOW +
                      "<--> Información del servicio <--> \n" + Fore.BLUE + "[♦]" + Fore.YELLOW +
                     " Nombre: " + Fore.GREEN + f"{name}  |   " + Fore.YELLOW + "Producto: " + Fore.GREEN + f"{product}"
                    + Fore.YELLOW + "  |  Versión: " + Fore.GREEN + f"{version}" + Fore.YELLOW + "|  Extra info: " +
                    Fore.GREEN + f"{extrainfo}" + Fore.YELLOW + "|  CPE:" + Fore.GREEN +
                   f"{cpe}  \n\nInfo: \n{script[0]}\n{script[1]}  \n")
                 print(Fore.GREEN + "\n"+"-" * 50, "\n")
 
+                text = f"""Puerto:  {p}/{state} \n<--> Información del servicio <--> \n
+    [♦] Nombre: {name}
+    Producto: {product}  
+    Versión: {version}   
+    Extra info: {extrainfo}    
+    CPE: {cpe}  \n\n
+    Info: \n{script[0]}\n{script[1]}  \n""" + "\n"+"-" * 50 + "\n"
+
+                write_file(f"[!] FOUND INFORMATION ABOUT SERVICE!!\n")
+                write_file(text)
+
         except KeyError:
             print(
                 Fore.CYAN + "Puerto: " + Fore.GREEN + f"{p}/{state} \n" + Fore.YELLOW +
                 "<--> Especificaciones del servicio <--> \n" + Fore.BLUE +
                 "[♦]" + Fore.YELLOW + " Nombre:" + Fore.GREEN + f"  {name}"
                                                                 "  |  " + Fore.YELLOW + "Producto:" + Fore.GREEN +
                 f" {product}    |  " + Fore.YELLOW + "Versión:" + Fore.GREEN + f" {version}  |  {extrainfo}  |  " +
                 Fore.YELLOW + "CPE:" + Fore.GREEN + f" {cpe} \n")
             print(Fore.GREEN + "\n" + "-" * 50)
 
+            text = f"""Puerto: {p}/{state} \n<--> Especificaciones del servicio <--> \n
+    [♦] Nombre: {name}    
+    Producto: {product}    
+    Versión: {version}  
+    Extra Info: {extrainfo}    
+    CPE: {cpe} \n""" + "\n" + "-" * 50 + "\n"
+
+            write_file(f"[!] FOUND INFORMATION ABOUT SERVICE!!\n")
+            write_file(text)
 
     if all_host is not None:
         if len(all_host) > 1:
             print(Fore.YELLOW + "OUTPUTS")
             for information in range(len(all_host)):
                 ids = all_host[information]['id']
                 if ids == "clock-skew":
@@ -738,22 +786,38 @@
                     print(Fore.GREEN + "\n" + "═" * 30 + "►", "\n")
 
     print_information(target, end_service_scan, init_scan_service, dict_serv)
 
 
 def print_information(target, end_service_scan, init_scan_service, dict_serv):
     # Tipo de sistema encontrado
-    ip = nm[target]['addresses']['ipv4']
-    ip_vendor = nm[target]['vendor']
-    if not ip_vendor:
+    try:
+        ip = nm[target]['addresses']['ipv4']
+    except Exception:
+        ip = "N/D"
+    try:
+        ip_vendor = nm[target]['vendor']
+    except Exception:
         ip_vendor = "N/D"
-    name_os = nm[target]['osmatch'][0]['name']
-    accuracy = nm[target]['osmatch'][0]['accuracy']
-    vendor = nm[target]['osmatch'][0]['osclass'][0]['vendor']
-    sys_cpe = nm[target]['osmatch'][0]['osclass'][0]['cpe'][0]
+    try:
+        name_os = nm[target]['osmatch'][0]['name']
+    except Exception:
+        name_os = "N/D"
+    try:
+        accuracy = nm[target]['osmatch'][0]['accuracy']
+    except Exception:
+        accuracy = "N/D"
+    try:
+        vendor = nm[target]['osmatch'][0]['osclass'][0]['vendor']
+    except Exception:
+        vendor = "N/D"
+    try:
+        sys_cpe = nm[target]['osmatch'][0]['osclass'][0]['cpe'][0]
+    except Exception:
+        sys_cpe = "N/D"
 
     def how_print():
         if ip_vendor == "N/D":
             return ip_vendor
         else:
             return [data for data in ip_vendor]
 
@@ -772,14 +836,19 @@
     print(Fore.GREEN + "═" * 50 + "►", "\n")
     print(Fore.BLUE + "MAC & Vendor " + Fore.YELLOW + "--> " + Fore.GREEN + f"{how_print()}")
 
     elapsed = (end_service_scan - init_scan_service)
     print(Fore.GREEN + "\n" + "-" * 50)
     print(Fore.GREEN + "Tiempo transcurrido duante el analisis -> {}".format(elapsed))
 
+    write_file("\nINFORMACIÓN DEL SISTEMA OBJETIVO" + "═" * 50 + "►" + "\n" + "SISTEMA -->" + f" {name_os}\n"
+               + "═" * 50 + "►" + "\n" + "Precisión --> " + f"{accuracy}\n" + "═" * 50 + "►" + "\n" + "Vendedor --> " +
+                            f"{vendor}\n" + "═" * 50 + "►" + "\n" + "CPE --> " + f"{sys_cpe}\n" + "═" * 50 + "►" + "\n" +
+               "IP --> " + f"{ip}\n" + "═" * 50 + "►" + "\n" + "MAC & Vendor --> " + f"{how_print()}")
+
     vlnsrch(dict_serv)
 
 
 def vlnsrch(dict_serv):
     # Analisis de vulners?
     while True:
         vuln = input(
@@ -1020,34 +1089,45 @@
 def write_file(text):
     userpath = get_user_path()
     location = userpath + "/Desktop/"
     filename = "scan.log"
 
     with open(location + filename, "a", encoding="utf-8") as log:
         now = str(time.ctime())
-        log.write("\n<<< " +now + " >>> " + text)
+        log.write("\n<<< " + now + " >>> " + text)
 
 
 def main():
     try:
-        text = """
-        PREPARING SCAN PORTS
-════════════════════════════════════\n"""
+        # Añadirmos el texto inicial en el archivo
+        text = "PREPARING SCAN PORTS\n" + "═" * 60 + "\n"
+
         # Creamos archivo y añadimos el inicio
         write_file(text)
+
         # Empezamos código limpiando pantalla
         clean()
+
         # Miramos si eres admin / root
         is_admin()
+
         # Verificamos NMAP
         verifi_tools()
+
         # Iniciamos la herramienta
         funcions()
 
     # Salida con CTRL + C
     except KeyboardInterrupt:
         print("\n\nSaliendo del programa...")
+
+        # Añadimos salida en el texto de salida
+        text = "EXITING PROGRAM...\n" + "═" * 60 + "\n"
+        write_file(text)
+
+        # Salimos del programa
         exit()
 
 
 if __name__ == "__main__":
+    # Ejecutamos la función principal
     main()
```

## Comparing `python_scan-0.4.4a2.dist-info/METADATA` & `python_scan-0.4.4a3.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-scan
-Version: 0.4.4a2
+Version: 0.4.4a3
 Summary: Herramienta para escaneo de puertos/vulners/explits en una IP
 Home-page: https://github.com/TownPablo/PORT_SCANNER
 Author: __TownPablo__
 Author-email: pablodiez024@proton.me
 License: MIT
 Keywords: port scan,seguridad,redes
 Description-Content-Type: text/markdown
@@ -14,15 +14,15 @@
 Requires-Dist: pyExploitDb (==0.2.9)
 Requires-Dist: pyfiglet (==0.8.post1)
 Requires-Dist: sockets (==1.0.0)
 Requires-Dist: python-nmap (==0.7.1)
 
 #                   PORT_SCANNER
 
-Autor: _TownPablo_ or _An0mal1a_
+Autor: _An0mal1a_
 
 
 
 #  --  Usabilidad 'PORT SCANNER' v0.4.4.a  --       
 
 Argumentos de la herramienta:
 
@@ -47,20 +47,23 @@
 
     3. Iniciamos una busqueda de vulnerabilidades públicas en dichos servicios...
 
     4. Tenemos la opcion de buscar en la base de datos de ExploitDb algún exploit público.
 
     5. Podemos abrir metasploit para utilziar la informacion recopilada
        anteriomente para lo que tengamos que hacer
-
     
     REQUISITOS:
             - NMAP
             - Metasploit (opcional)
-            
+    ---------------------------------------------------------------------------------------------------        
+    Se han añadido funciones para crear un archivo 'scan.log' en el escritorio.
+    Se han añadido Host Discovery y Os_guess que en base el ttl no dice de forma simple el OS que corre 
+    Se han corregido errores
+    En mejora argumentos personalizados de "NMAP"
 
 
 # Pip:
 
     command_line = pip install python-scan
 
 # Git:
```

