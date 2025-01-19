# kcsc-2025-write-up

I. Reverse engineering.
- Hidden (incomplete and/or incorrect): used wine command.
![Screenshot_2025-01-18_11_56_57](https://github.com/user-attachments/assets/61a58597-8e5b-4fef-aca3-ea0599810a3a)

- easyre (incomplete):
  + Attempt 1: gdb -> info func -> ...nothing.
![Screenshot_2025-01-19_19_34_18](https://github.com/user-attachments/assets/3d54e801-e620-432f-a681-4efc8d257837)

  + Attempt 2: wine. -> nothing.

II. PWN.
- AAA:
  + some clues that might be necessary(?): Exposed 1337 TCP, WORKDIR /home/main, ADD ./flag /, ADD ./main /home/main.
  + maybe this task needs to be solve with socat?
  + User input returns the same so might need to use some sort of injection?

III. Forensics.
- Powershell 101:
![Screenshot_2025-01-19_19_57_56](https://github.com/user-attachments/assets/6a725484-5e6e-4f38-a075-d07109bf9870)
  + used pwsh.
  + converted the base64 code(not sure if it's relevant, but worth a try.):
    ![Screenshot_2025-01-19_20_00_32](https://github.com/user-attachments/assets/40911a73-1265-45a6-8eb5-1e034820b2c3)
