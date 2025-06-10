 UDP-File-Transfer
 
Setup Instructions

1. Requirements
   
- Python 3.x
- tkinter (built-in)
Install requirements (if needed):
pip install tk

2. Project Structure
udp_file_transfer

udp_file_transfer_gui.py # Main GUI application
 sender.py # Sends files over UDP
 receiver.py # Receives files over UDP
 README.md # Documentation
3. Running the App
python udp_file_transfer_gui.py

Code Overview

- sender.py: Sends file over UDP in chunks, with progress tracking.
- receiver.py: Listens for incoming file, reconstructs with original filename.
- udp_file_transfer_gui.py: GUI with file queue, progress, pause, resume, cancel, and retry.
  
Functions used:

send_file(file_path, ip, port, progress_callback)
receive_file(save_dir, port, progress_callback)

User Manual

Sending Files:

1. Add Files
2. Enter Receiver IP and Port (e.g. 5005)
3. Start Sending
4. Use Pause, Resume, Cancel, Retry as needed
   
Receiving Files:

1. Enter Port
2. Choose Save Folder & Receive
3. File is saved with original name

   
Tips

- Use same network for sender and receiver.
- UDP is fast but not reliable. Use retry feature.
- For full reliability, consider switching to TCP

  
