# Comparing `tmp/heyoo-0.0.8-py3-none-any.whl.zip` & `tmp/heyoo-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 9648 bytes, number of entries: 6
--rw-rw-r--  2.0 unx    34144 b- defN 23-Feb-01 17:34 heyoo/__init__.py
--rw-rw-r--  2.0 unx     1066 b- defN 23-Feb-01 17:57 heyoo-0.0.8.dist-info/LICENSE
--rw-rw-r--  2.0 unx     7540 b- defN 23-Feb-01 17:57 heyoo-0.0.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Feb-01 17:57 heyoo-0.0.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx        6 b- defN 23-Feb-01 17:57 heyoo-0.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      450 b- defN 23-Feb-01 17:57 heyoo-0.0.8.dist-info/RECORD
-6 files, 43298 bytes uncompressed, 8838 bytes compressed:  79.6%
+Zip file size: 12408 bytes, number of entries: 6
+-rw-rw-r--  2.0 unx    38308 b- defN 23-May-14 19:58 heyoo/__init__.py
+-rw-rw-r--  2.0 unx     1066 b- defN 23-May-14 20:00 heyoo-0.0.9.dist-info/LICENSE
+-rw-rw-r--  2.0 unx    15573 b- defN 23-May-14 20:00 heyoo-0.0.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-14 20:00 heyoo-0.0.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        6 b- defN 23-May-14 20:00 heyoo-0.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      451 b- defN 23-May-14 20:00 heyoo-0.0.9.dist-info/RECORD
+6 files, 55496 bytes uncompressed, 11598 bytes compressed:  79.1%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: heyoo/__init__.py
 Comment: 
 
-Filename: heyoo-0.0.8.dist-info/LICENSE
+Filename: heyoo-0.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: heyoo-0.0.8.dist-info/METADATA
+Filename: heyoo-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: heyoo-0.0.8.dist-info/WHEEL
+Filename: heyoo-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: heyoo-0.0.8.dist-info/top_level.txt
+Filename: heyoo-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: heyoo-0.0.8.dist-info/RECORD
+Filename: heyoo-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## heyoo/__init__.py

```diff
@@ -2,25 +2,22 @@
 Unofficial python wrapper for the WhatsApp Cloud API.
 """
 from __future__ import annotations
 import os
 import mimetypes
 import requests
 import logging
+import warnings
+from colorama import Fore, Style
 from requests_toolbelt.multipart.encoder import MultipartEncoder
 from typing import Optional, Dict, Any, List, Union, Tuple, Callable
 
 
 # Setup logging
-
-logging.basicConfig(
-    level=logging.INFO,
-    format="%(asctime)s - %(name)s - %(levelname)s - %(message)s",
-)
-
+logging.getLogger(__name__).addHandler(logging.NullHandler())
 
 class WhatsApp(object):
     """ "
     WhatsApp Object
     """
 
     def __init__(self, token=None, phone_number_id=None):
@@ -72,15 +69,15 @@
         logging.info(f"Sending message to {recipient_id}")
         r = requests.post(f"{self.url}", headers=self.headers, json=data)
         if r.status_code == 200:
             logging.info(f"Message sent to {recipient_id}")
             return r.json()
         logging.info(f"Message not sent to {recipient_id}")
         logging.info(f"Status code: {r.status_code}")
-        logging.info(f"Response: {r.json()}")
+        logging.error(f"Response: {r.json()}")
         return r.json()
 
     def reply_to_message(
         self, message_id: str, recipient_id: str, message: str, preview_url: bool = True
     ):
         """
         Replies to a message
@@ -103,62 +100,36 @@
         logging.info(f"Replying to {message_id}")
         r = requests.post(f"{self.url}", headers=self.headers, json=data)
         if r.status_code == 200:
             logging.info(f"Message sent to {recipient_id}")
             return r.json()
         logging.info(f"Message not sent to {recipient_id}")
         logging.info(f"Status code: {r.status_code}")
-        logging.info(f"Response: {r.json()}")
+        logging.error(f"Response: {r.json()}")
         return r.json()
 
-    def send_template(self, template: str, recipient_id: str, recipient_type="individual",
-                        lang: str = "en_US", components: List = None):  
-            """
-            Sends a template message to a WhatsApp user, Template messages can either be;
-                1. Text template
-                2. Media based template
-                3. Interactive template
-            You can customize the template message by passing a dictionary of components.
-            You can find the available components in the documentation.
-            https://developers.facebook.com/docs/whatsapp/cloud-api/guides/send-message-templates
-            Args:
-                template[str]: Template name to be sent to the user
-                recipient_id[str]: Phone number of the user with country code wihout +
-                lang[str]: Language of the template message
-                components[list]: List of components to be sent to the user  # CHANGE
-            Example:
-                >>> from whatsapp import WhatsApp
-                >>> whatsapp = WhatsApp(token, phone_number_id)
-                >>> whatsapp.send_template("hello_world", "5511999999999", lang="en_US"))
-            """
-            if components is None:  # TO NOT USE LIST AS DEFAULT, BECAUSE IT IS MUTABLE
-                components = []
-            data = {
-                "messaging_product": "whatsapp",
-                "recipient_type": recipient_type,
-                "to": recipient_id,
-                "type": "template",
-                "template": {
-                    "name": template,
-                    "language": {"code": lang},
-                    "components": components,
-                },
-            }
-            logging.info(f"Sending template to {recipient_id}")
-            r = requests.post(self.url, headers=self.headers, json=data)
-
-            if r.status_code == 200:
-                logging.info(f"Template sent to {recipient_id}")
-                return r.json()
-            logging.info(f"Template not sent to {recipient_id}")
-            logging.info(f"Status code: {r.status_code}")
-            logging.info(f"Response: {r.json()}")
-            return r.json()
-
-    def send_templatev2(self, template, recipient_id, components, lang="en_US"):
+    def send_template(self, template, recipient_id, components, lang: str = "en_US"):
+        """
+        Sends a template message to a WhatsApp user, Template messages can either be;
+            1. Text template
+            2. Media based template
+            3. Interactive template
+        You can customize the template message by passing a dictionary of components.
+        You can find the available components in the documentation.
+        https://developers.facebook.com/docs/whatsapp/cloud-api/guides/send-message-templates
+        Args:
+            template[str]: Template name to be sent to the user
+            recipient_id[str]: Phone number of the user with country code wihout +
+            lang[str]: Language of the template message
+            components[list]: List of components to be sent to the user  # CHANGE
+        Example:
+            >>> from whatsapp import WhatsApp
+            >>> whatsapp = WhatsApp(token, phone_number_id)
+            >>> whatsapp.send_template("hello_world", "5511999999999", lang="en_US"))
+        """
         data = {
             "messaging_product": "whatsapp",
             "to": recipient_id,
             "type": "template",
             "template": {
                 "name": template,
                 "language": {"code": lang},
@@ -168,17 +139,23 @@
         logging.info(f"Sending template to {recipient_id}")
         r = requests.post(self.url, headers=self.headers, json=data)
         if r.status_code == 200:
             logging.info(f"Template sent to {recipient_id}")
             return r.json()
         logging.info(f"Template not sent to {recipient_id}")
         logging.info(f"Status code: {r.status_code}")
-        logging.info(f"Response: {r.json()}")
+        logging.error(f"Response: {r.json()}")
         return r.json()
 
+    def send_templatev2(self, template, recipient_id, components, lang: str = "en_US"):
+        message = f"{Fore.RED}The 'send_templatev2' method is being deprecated and will be removed in the future. Please use the 'send_template' method instead.{Style.RESET_ALL}"
+        warnings.warn(message, DeprecationWarning)
+        return send_template(template, recipient_id, components, lang=lang)
+    
+    
     def send_location(self, lat, long, name, address, recipient_id):
         """
         Sends a location message to a WhatsApp user
 
         Args:
             lat[str]: Latitude of the location
             long[str]: Longitude of the location
@@ -261,16 +238,58 @@
             logging.info(f"Image sent to {recipient_id}")
             return r.json()
         logging.info(f"Image not sent to {recipient_id}")
         logging.info(f"Status code: {r.status_code}")
         logging.error(r.json())
         return r.json()
 
-    def send_sticker(self, sticker: str, recipient_id: str, linl=True):
-        pass
+    def send_sticker(self, sticker: str, recipient_id: str, recipient_type="individual", link=True):
+        """
+        Sends a sticker message to a WhatsApp user
+
+        There are two ways to send a sticker message to a user, either by passing the image id or by passing the sticker link.
+        Sticker id is the id of the sticker uploaded to the cloud api.
+
+        Args:
+            sticker[str]: Sticker id or link of the sticker
+            recipient_id[str]: Phone number of the user with country code wihout +
+            recipient_type[str]: Type of the recipient, either individual or group
+            link[bool]: Whether to send an sticker id or an sticker link, True means that the sticker is an id, False means that the image is a link
+
+
+        Example:
+            >>> from whatsapp import WhatsApp
+            >>> whatsapp = WhatsApp(token, phone_number_id)
+            >>> whatsapp.send_sticker("170511049062862", "5511999999999", link=False)
+        """
+        if link:
+            data = {
+                "messaging_product": "whatsapp",
+                "recipient_type": recipient_type,
+                "to": recipient_id,
+                "type": "sticker",
+                "sticker": {"link": sticker},
+            }
+        else:
+            data = {
+                "messaging_product": "whatsapp",
+                "recipient_type": recipient_type,
+                "to": recipient_id,
+                "type": "sticker",
+                "sticker": {"id": sticker},
+            }
+        logging.info(f"Sending sticker to {recipient_id}")
+        r = requests.post(self.url, headers=self.headers, json=data)
+        if r.status_code == 200:
+            logging.info(f"Sticker sent to {recipient_id}")
+            return r.json()
+        logging.info(f"Sticker not sent to {recipient_id}")
+        logging.info(f"Status code: {r.status_code}")
+        logging.error(r.json())
+        return r.json()
 
     def send_audio(self, audio, recipient_id, link=True):
         """
         Sends an audio message to a WhatsApp user
         Audio messages can either be sent by passing the audio id or by passing the audio link.
 
         Args:
@@ -303,15 +322,17 @@
             logging.info(f"Audio sent to {recipient_id}")
             return r.json()
         logging.info(f"Audio not sent to {recipient_id}")
         logging.info(f"Status code: {r.status_code}")
         logging.error(f"Response: {r.json()}")
         return r.json()
 
-    def send_video(self, video, recipient_id, caption=None, link=True):
+    def send_video(
+        self, video, recipient_id, caption=None, link=True
+    ) -> Dict[Any, Any]:
         """ "
         Sends a video message to a WhatsApp user
         Video messages can either be sent by passing the video id or by passing the video link.
 
         Args:
             video[str]: Video id or link of the video
             recipient_id[str]: Phone number of the user with country code wihout +
@@ -343,15 +364,50 @@
             logging.info(f"Video sent to {recipient_id}")
             return r.json()
         logging.info(f"Video not sent to {recipient_id}")
         logging.info(f"Status code: {r.status_code}")
         logging.error(f"Response: {r.json()}")
         return r.json()
 
-    def send_document(self, document, recipient_id, caption=None, link=True):
+    def send_custom_json(self, data, recipient_id=None):
+        """
+        Sends a custom json to a WhatsApp user. This can be used to send custom objects to the message endpoint.
+
+        Args:
+            data[dict]: Dictionary that should be send
+            recipient_id[str]: Phone number of the user with country code wihout +
+        Example:
+            >>> from whatsapp import WhatsApp
+            >>> whatsapp = WhatsApp(token, phone_number_id)
+            >>> whatsapp.send_custom_json({
+                    "messaging_product": "whatsapp",
+                    "type": "audio",
+                    "audio": {"id": audio}}, "5511999999999")
+        """
+
+        if recipient_id:
+            if "to" in data.keys():
+                data_recipient_id = data["to"]
+                logging.info(f"Recipient Id is defined in data ({data_recipient_id}) and recipient_id parameter ({recipient_id})")
+            else:
+                data["to"] = recipient_id
+
+        logging.info(f"Sending custom json to {recipient_id}")
+        r = requests.post(self.url, headers=self.headers, json=data)
+        if r.status_code == 200:
+            logging.info(f"Custom json sent to {recipient_id}")
+            return r.json()
+        logging.info(f"Custom json not sent to {recipient_id}")
+        logging.info(f"Status code: {r.status_code}")
+        logging.error(f"Response: {r.json()}")
+        return r.json()
+
+    def send_document(
+        self, document, recipient_id, caption=None, link=True
+    ) -> Dict[Any, Any]:
         """ "
         Sends a document message to a WhatsApp user
         Document messages can either be sent by passing the document id or by passing the document link.
 
         Args:
             document[str]: Document id or link of the document
             recipient_id[str]: Phone number of the user with country code wihout +
@@ -384,15 +440,17 @@
             logging.info(f"Document sent to {recipient_id}")
             return r.json()
         logging.info(f"Document not sent to {recipient_id}")
         logging.info(f"Status code: {r.status_code}")
         logging.error(f"Response: {r.json()}")
         return r.json()
 
-    def send_contacts(self, contacts: List[Dict[Any, Any]], recipient_id: str):
+    def send_contacts(
+        self, contacts: List[Dict[Any, Any]], recipient_id: str
+    ) -> Dict[Any, Any]:
         """send_contacts
 
         Send a list of contacts to a user
 
         Args:
             contacts(List[Dict[Any, Any]]): List of contacts to send
             recipient_id(str): Phone number of the user with country code wihout +
@@ -429,15 +487,15 @@
             logging.info(f"Contacts sent to {recipient_id}")
             return r.json()
         logging.info(f"Contacts not sent to {recipient_id}")
         logging.info(f"Status code: {r.status_code}")
         logging.error(f"Response: {r.json()}")
         return r.json()
 
-    def upload_media(self, media: str):
+    def upload_media(self, media: str) -> Union[Dict[Any, Any], None]:
         """
         Uploads a media to the cloud api and returns the id of the media
 
         Args:
             media[str]: Path of the media to be uploaded
 
         Example:
@@ -470,15 +528,15 @@
             logging.info(f"Media {media} uploaded")
             return r.json()
         logging.info(f"Error uploading media {media}")
         logging.info(f"Status code: {r.status_code}")
         logging.info(f"Response: {r.json()}")
         return None
 
-    def delete_media(self, media_id: str):
+    def delete_media(self, media_id: str) -> Union[Dict[Any, Any], None]:
         """
         Deletes a media from the cloud api
 
         Args:
             media_id[str]: Id of the media to be deleted
         """
         logging.info(f"Deleting media {media_id}")
@@ -486,37 +544,55 @@
         if r.status_code == 200:
             logging.info(f"Media {media_id} deleted")
             return r.json()
         logging.info(f"Error deleting media {media_id}")
         logging.info(f"Status code: {r.status_code}")
         logging.info(f"Response: {r.json()}")
         return None
-    
-    def mark_as_read(self, message_id: str):
+
+    def mark_as_read(self, message_id: str) -> Dict[Any, Any]:
         """
         Marks a message as read
-        
-        Args: 
+
+        Args:
             message_id[str]: Id of the message to be marked as read
+
+        Returns:
+            Dict[Any, Any]: Response from the API
+
+        Example:
+            >>> from whatsapp import WhatsApp
+            >>> whatsapp = WhatsApp(token, phone_number_id)
+            >>> whatsapp.mark_as_read("message_id")
         """
         headers = {
-            'Authorization': f'Bearer {self.token}',
-            'Content-Type': 'application/json',
+            "Authorization": f"Bearer {self.token}",
+            "Content-Type": "application/json",
         }
 
         json_data = {
-            'messaging_product': 'whatsapp',
-            'status': 'read',
-            'message_id': message_id,
+            "messaging_product": "whatsapp",
+            "status": "read",
+            "message_id": message_id,
         }
+        logging.info(f"Marking message {message_id} as read")
         response = requests.post(
-            f'{self.v15_base_url}/{self.phone_number_id}/messages', headers=headers, json=json_data).json()
-        return response["success"]
+            f"{self.v15_base_url}/{self.phone_number_id}/messages",
+            headers=headers,
+            json=json_data,
+        ).json()
+        if response.status_code == 200:
+            logging.info(f"Message {message_id} marked as read")
+            return response
+        logging.info(f"Error marking message {message_id} as read")
+        logging.info(f"Status code: {response.status_code}")
+        logging.info(f"Response: {response.json()}")
+        return response
 
-    def create_button(self, button):
+    def create_button(self, button: Dict[Any, Any]) -> Dict[Any, Any]:
         """
         Method to create a button object to be used in the send_message method.
 
         This is method is designed to only be used internally by the send_button method.
 
         Args:
                button[dict]: A dictionary containing the button data
@@ -526,15 +602,15 @@
             data["header"] = {"type": "text", "text": button.get("header")}
         if button.get("body"):
             data["body"] = {"text": button.get("body")}
         if button.get("footer"):
             data["footer"] = {"text": button.get("footer")}
         return data
 
-    def send_button(self, button, recipient_id):
+    def send_button(self, button: Dict[Any, Any], recipient_id: str) -> Dict[Any, Any]:
         """
         Sends an interactive buttons message to a WhatsApp user
 
         Args:
             button[dict]: A dictionary containing the button data(rows-title may not exceed 20 characters)
             recipient_id[str]: Phone number of the user with country code wihout +
 
@@ -552,15 +628,17 @@
             logging.info(f"Buttons sent to {recipient_id}")
             return r.json()
         logging.info(f"Buttons not sent to {recipient_id}")
         logging.info(f"Status code: {r.status_code}")
         logging.info(f"Response: {r.json()}")
         return r.json()
 
-    def send_reply_button(self, button, recipient_id):
+    def send_reply_button(
+        self, button: Dict[Any, Any], recipient_id: str
+    ) -> Dict[Any, Any]:
         """
         Sends an interactive reply buttons[menu] message to a WhatsApp user
 
         Args:
             button[dict]: A dictionary containing the button data
             recipient_id[str]: Phone number of the user with country code wihout +
 
@@ -579,15 +657,15 @@
             logging.info(f"Reply buttons sent to {recipient_id}")
             return r.json()
         logging.info(f"Reply buttons not sent to {recipient_id}")
         logging.info(f"Status code: {r.status_code}")
         logging.info(f"Response: {r.json()}")
         return r.json()
 
-    def query_media_url(self, media_id: str):
+    def query_media_url(self, media_id: str) -> Union[str, None]:
         """
         Query media url from media id obtained either by manually uploading media or received media
 
         Args:
             media_id[str]: Media id of the media
 
         Returns:
@@ -605,15 +683,17 @@
             logging.info(f"Media url queried for {media_id}")
             return r.json()["url"]
         logging.info(f"Media url not queried for {media_id}")
         logging.info(f"Status code: {r.status_code}")
         logging.info(f"Response: {r.json()}")
         return None
 
-    def download_media(self, media_url: str, mime_type: str, file_path: str = "temp"):
+    def download_media(
+        self, media_url: str, mime_type: str, file_path: str = "temp"
+    ) -> Union[str, None]:
         """
         Download media from media url obtained either by manually uploading media or received media
 
         Args:
             media_url[str]: Media url of the media
             mime_type[str]: Mime type of the media
             file_path[str]: Path of the file to be downloaded to. Default is "temp"
@@ -638,30 +718,45 @@
                 f"{file_path}.{extension}" if file_path else f"temp.{extension}"
             )
             with open(save_file_here, "wb") as f:
                 f.write(content)
             logging.info(f"Media downloaded to {save_file_here}")
             return f.name
         except Exception as e:
-            print(e)
-            logging.info(f"Error downloading media to {save_file_here}")
+            logging.info(e)
+            logging.ERROR(f"Error downloading media to {save_file_here}")
             return None
 
-    def preprocess(self, data):
+    def preprocess(self, data: Dict[Any, Any]) -> Dict[Any, Any]:
         """
         Preprocesses the data received from the webhook.
 
         This method is designed to only be used internally.
 
         Args:
             data[dict]: The data received from the webhook
         """
         return data["entry"][0]["changes"][0]["value"]
 
-    def get_mobile(self, data)-> Union[str, None]:
+    def is_message(self, data: Dict[Any, Any]) -> bool:
+        """is_message checks if the data received from the webhook is a message.
+
+        Args:
+            data (Dict[Any, Any]): The data received from the webhook
+
+        Returns:
+            bool: True if the data is a message, False otherwise
+        """
+        data = self.preprocess(data)
+        if "messages" in data:
+            return True
+        else:
+            return False
+
+    def get_mobile(self, data: Dict[Any, Any]) -> Union[str, None]:
         """
         Extracts the mobile number of the sender from the data received from the webhook.
 
         Args:
             data[dict]: The data received from the webhook
         Returns:
             str: The mobile number of the sender
@@ -671,15 +766,15 @@
             >>> whatsapp = WhatsApp(token, phone_number_id)
             >>> mobile = whatsapp.get_mobile(data)
         """
         data = self.preprocess(data)
         if "contacts" in data:
             return data["contacts"][0]["wa_id"]
 
-    def get_name(self, data)-> Union[str, None]:
+    def get_name(self, data: Dict[Any, Any]) -> Union[str, None]:
         """
         Extracts the name of the sender from the data received from the webhook.
 
         Args:
             data[dict]: The data received from the webhook
         Returns:
             str: The name of the sender
@@ -688,15 +783,15 @@
             >>> whatsapp = WhatsApp(token, phone_number_id)
             >>> mobile = whatsapp.get_name(data)
         """
         contact = self.preprocess(data)
         if contact:
             return contact["contacts"][0]["profile"]["name"]
 
-    def get_message(self, data)-> Union[str, None]:
+    def get_message(self, data: Dict[Any, Any]) -> Union[str, None]:
         """
         Extracts the text message of the sender from the data received from the webhook.
 
         Args:
             data[dict]: The data received from the webhook
         Returns:
             str: The text message received from the sender
@@ -705,15 +800,15 @@
             >>> whatsapp = WhatsApp(token, phone_number_id)
             >>> message = message.get_message(data)
         """
         data = self.preprocess(data)
         if "messages" in data:
             return data["messages"][0]["text"]["body"]
 
-    def get_message_id(self, data)-> Union[str, None]:
+    def get_message_id(self, data: Dict[Any, Any]) -> Union[str, None]:
         """
         Extracts the message id of the sender from the data received from the webhook.
 
         Args:
             data[dict]: The data received from the webhook
         Returns:
             str: The message id of the sender
@@ -722,15 +817,15 @@
             >>> whatsapp = WhatsApp(token, phone_number_id)
             >>> message_id = whatsapp.get_message_id(data)
         """
         data = self.preprocess(data)
         if "messages" in data:
             return data["messages"][0]["id"]
 
-    def get_message_timestamp(self, data)-> Union[str, None]:
+    def get_message_timestamp(self, data: Dict[Any, Any]) -> Union[str, None]:
         """ "
         Extracts the timestamp of the message from the data received from the webhook.
 
         Args:
             data[dict]: The data received from the webhook
         Returns:
             str: The timestamp of the message
@@ -739,37 +834,37 @@
             >>> whatsapp = WhatsApp(token, phone_number_id)
             >>> whatsapp.get_message_timestamp(data)
         """
         data = self.preprocess(data)
         if "messages" in data:
             return data["messages"][0]["timestamp"]
 
-    def get_interactive_response(self, data)-> Union[Dict, None]:
+    def get_interactive_response(self, data: Dict[Any, Any]) -> Union[Dict, None]:
         """
          Extracts the response of the interactive message from the data received from the webhook.
 
          Args:
             data[dict]: The data received from the webhook
         Returns:
             dict: The response of the interactive message
 
         Example:
             >>> from whatsapp import WhatsApp
             >>> whatsapp = WhatsApp(token, phone_number_id)
             >>> response = whatsapp.get_interactive_response(data)
-            >>> intractive_type = response.get("type")
-            >>> message_id = response[intractive_type]["id"]
-            >>> message_text = response[intractive_type]["title"]
+            >>> interactive_type = response.get("type")
+            >>> message_id = response[interactive_type]["id"]
+            >>> message_text = response[interactive_type]["title"]
         """
         data = self.preprocess(data)
         if "messages" in data:
             if "interactive" in data["messages"][0]:
                 return data["messages"][0]["interactive"]
 
-    def get_location(self, data)-> Union[Dict, None]:
+    def get_location(self, data: Dict[Any, Any]) -> Union[Dict, None]:
         """
         Extracts the location of the sender from the data received from the webhook.
 
         Args:
             data[dict]: The data received from the webhook
 
         Returns:
@@ -781,15 +876,15 @@
             >>> whatsapp.get_location(data)
         """
         data = self.preprocess(data)
         if "messages" in data:
             if "location" in data["messages"][0]:
                 return data["messages"][0]["location"]
 
-    def get_image(self, data)-> Union[Dict, None]:
+    def get_image(self, data: Dict[Any, Any]) -> Union[Dict, None]:
         """ "
         Extracts the image of the sender from the data received from the webhook.
 
         Args:
             data[dict]: The data received from the webhook
         Returns:
             dict: The image_id of an image sent by the sender
@@ -799,16 +894,16 @@
             >>> whatsapp = WhatsApp(token, phone_number_id)
             >>> image_id = whatsapp.get_image(data)
         """
         data = self.preprocess(data)
         if "messages" in data:
             if "image" in data["messages"][0]:
                 return data["messages"][0]["image"]
-     
-    def get_document(self, data)-> Union[Dict, None]:
+
+    def get_document(self, data: Dict[Any, Any]) -> Union[Dict, None]:
         """ "
         Extracts the document of the sender from the data received from the webhook.
 
         Args:
             data[dict]: The data received from the webhook
         Returns:
             dict: The document_id of an image sent by the sender
@@ -819,16 +914,15 @@
             >>> document_id = whatsapp.get_document(data)
         """
         data = self.preprocess(data)
         if "messages" in data:
             if "document" in data["messages"][0]:
                 return data["messages"][0]["document"]
 
-
-    def get_audio(self, data)-> Union[Dict, None]:
+    def get_audio(self, data: Dict[Any, Any]) -> Union[Dict, None]:
         """
         Extracts the audio of the sender from the data received from the webhook.
 
         Args:
             data[dict]: The data received from the webhook
 
         Returns:
@@ -840,15 +934,15 @@
             >>> whatsapp.get_audio(data)
         """
         data = self.preprocess(data)
         if "messages" in data:
             if "audio" in data["messages"][0]:
                 return data["messages"][0]["audio"]
 
-    def get_video(self, data)-> Union[Dict, None]:
+    def get_video(self, data: Dict[Any, Any]) -> Union[Dict, None]:
         """
         Extracts the video of the sender from the data received from the webhook.
 
         Args:
             data[dict]: The data received from the webhook
 
         Returns:
@@ -860,15 +954,15 @@
             >>> whatsapp.get_video(data)
         """
         data = self.preprocess(data)
         if "messages" in data:
             if "video" in data["messages"][0]:
                 return data["messages"][0]["video"]
 
-    def get_message_type(self, data)-> Union[str, None]:
+    def get_message_type(self, data: Dict[Any, Any]) -> Union[str, None]:
         """
         Gets the type of the message sent by the sender from the data received from the webhook.
 
 
         Args:
             data [dict]: The data received from the webhook
 
@@ -880,28 +974,28 @@
             >>> whatsapp = WhatsApp(token, phone_number_id)
             >>> whatsapp.get_message_type(data)
         """
         data = self.preprocess(data)
         if "messages" in data:
             return data["messages"][0]["type"]
 
-    def get_delivery(self, data)-> Union[Dict, None]:
+    def get_delivery(self, data: Dict[Any, Any]) -> Union[Dict, None]:
         """
         Extracts the delivery status of the message from the data received from the webhook.
         Args:
             data [dict]: The data received from the webhook
 
         Returns:
             dict: The delivery status of the message and message id of the message
         """
         data = self.preprocess(data)
         if "statuses" in data:
             return data["statuses"][0]["status"]
 
-    def changed_field(self, data):
+    def changed_field(self, data: Dict[Any, Any]) -> str:
         """
         Helper function to check if the field changed in the data received from the webhook.
 
         Args:
             data [dict]: The data received from the webhook
 
         Returns:
```

## Comparing `heyoo-0.0.8.dist-info/LICENSE` & `heyoo-0.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

