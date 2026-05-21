# Mach-Card
Mach Card is a custom NFC-enabled PCB business card that transmits a URL on tap and lights up an LED all powered wirelessly from your phone.

What
Mach Card is a custom NFC-enabled PCB business card. Tap it to any NFC-enabled phone and it instantly transmits a URL. It also lights up an LED, all without a battery or any power source.

Why
I wanted a way to share my links and contact info that felt personal and technical at the same time. A paper business card felt boring. So I designed this as a way to learn PCB design while making something I'd actually use and hand out.

How
The card is built around the NT3H2111 NFC chip, which harvests energy wirelessly from a phone's NFC radio field. That harvested power runs through a 220nF capacitor to the chip's VOUT pin, which drives a LED through a 47Ω current limiting resistor. A PCB trace antenna loop handles both communication and energy harvesting.

<img width="744" height="362" alt="Screenshot 2026-05-21 161924" src="https://github.com/user-attachments/assets/8470d410-067d-4975-9adb-7522fd73ca55" />
<img width="648" height="352" alt="Screenshot 2026-05-21 161918" src="https://github.com/user-attachments/assets/449fa6aa-16df-4700-bcc3-ddc2c3f0e131" />
<img width="1407" height="488" alt="Screenshot 2026-05-21 173339" src="https://github.com/user-attachments/assets/0bc8ec60-14cf-490c-9ceb-2f971c53b046" />
