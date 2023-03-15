# NTU_notes

- Download VirtualBox
    - Windows https://gigamove.rwth-aachen.de/de/download/2a7387f22c61e4a2992ec0016fc4489b
    - Mac https://gigamove.rwth-aachen.de/de/download/13228e355364060b7f7ba804210b8d74
- Enable virtualization in BIOS, google this if you don't know what this is
- Download VM file: https://gigamove.rwth-aachen.de/de/download/0ed71e4b7f5c4e40b1fc38e1247c8812


YouTube lectures: https://www.youtube.com/channel/UCPv4f5pMBkKm1Pvek3Ep0sA

Yahtzee code: https://github.com/alxhoff/empty-c-project/tree/yahtzee

Emulator Documentation: https://alxhoff.github.io/FreeRTOS-Emulator/

FreeRTOS Documentation: https://www.freertos.org/a00125.html

## Exercise

Create two tasks, task 1 (use vDemoTask1) is created with a higher priority than task 2 (create this task), task 1 signals task 2 with a semaphore (task 2 blocks waiting for this) to wake up and increment a locked (mutex) global variable which is then sent back to task 1, using a queue, which is waiting for this value.