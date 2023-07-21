# Website-Blocker-Using-Python
 The provided code is a simple Python program that creates a graphical user interface (GUI) using the Tkinter library for blocking and unblocking websites on a local machine. 
 It allows the user to input website addresses, which will be blocked or unblocked by modifying the hosts file on the Windows system.

# Code Explanation: 

Importing Tkinter: 
The code starts by importing the Tk class and other necessary components from the tkinter module.

GUI Setup: 
The code creates a window with a specific size, title, and heading label using the Label and geometry methods.

Website Input: 
A label and a Text widget are provided for the user to enter website addresses to block or unblock.

Blocking Function (Blocker): 
The Blocker function is responsible for blocking the entered websites. It reads the current content of the hosts file, checks if the websites are already blocked, and writes the IP address and website to the hosts file if they are not already present. Appropriate messages are displayed using Label widgets to inform the user if the website is already blocked or has been successfully blocked.

Unblocking Function (Unblock): 
The Unblock function is responsible for unblocking the entered websites. It reads the current content of the hosts file, removes the blocked websites, and writes the updated content back to the file. Appropriate messages are displayed to inform the user if the website is already unblocked or has been successfully unblocked.

Block and Unblock Buttons: 
Two buttons, "Block" and "Unblock," are provided to trigger the respective actions when clicked. They are linked to the Blocker and Unblock functions, respectively.

mainloop():
The mainloop() method is called to run the Tkinter event loop, which keeps the GUI responsive and allows the user to interact with it.

Please note that modifying the hosts file requires administrative privileges on most systems, 
so the program may need to be run with administrative rights for the blocking and unblocking to work correctly. 
Additionally, the code provided is specific to Windows systems due to the path used for the hosts file. It may need adjustments for other operating systems.

Overall, this program provides a basic website blocker tool, but keep in mind that it is limited to blocking/unblocking websites on the local machine. 
In a real-world scenario, you would need more sophisticated methods, such as DNS filtering or using network-level firewalls, 
to block websites effectively across an entire network.



