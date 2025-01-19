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
![Screenshot_2025-01-19_19_34_18](https://github.com/user-attachments/assets/eff32513-8c3c-446b-bbd8-dcfdb74eb390)

  + some clues that might be necessary(?): Exposed 1337 TCP, WORKDIR /home/main, ADD ./flag /, ADD ./main /home/main.
  + maybe this task needs to be solve with socat?
  + User input returns the same so might need to use some sort of injection?
