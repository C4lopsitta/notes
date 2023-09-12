# To do
- [ ] Add threads to application
- [ ] Make I/O thread for Keyboard reading from native device file
> [!NOTE]- How i wanna make this
> **Function set to implement**
> - Read next keystroke (any)
> - Read next character keystroke
> - Read character string, terminating with '\n'
> - Read character string, up to *n* characters, terminating with '\n'
> - Read character string, until *n* characters have been read
> **Possible ideas to implement**
> - Sending interrupts to main thread when specific keystrokes are sent
> 	- Registering those keystrokes with an appropriate function
> - Reading modifier keystrokes
> - Reading keystrokes combinations
- [ ] Add sockets for multiplayer on local network
- [ ] Add harder AI