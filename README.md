# Mach-Card

Mach Card is a custom NFC-enabled PCB business card that transmits a URL on tap and lights up an LED all powered wirelessly from your phone.

What
Mach Card is a custom NFC-enabled PCB business card. Tap it to any NFC-enabled phone and it instantly transmits a URL. It also lights up an LED, all without a battery or any power source.

Why
I wanted a way to share my links and contact info that felt personal and technical at the same time. A paper business card felt boring. So I designed this as a way to learn PCB design while making something I'd actually use and hand out.

How
The card is built around the NT3H2111 NFC chip, which harvests energy wirelessly from a phone's NFC radio field. That harvested power runs through a 220nF capacitor to the chip's VOUT pin, which drives a LED through a 47Ω current limiting resistor. A PCB trace antenna loop handles both communication and energy harvesting. The board was designed in [EasyEDA](https://easyeda.com/)
, and manufactured and assembled by [JLCPCB](https://jlcpcb.com/)
.

How It All Fits Together
The antenna loop, chip, resistor, capacitor, and LED are all on one 88.9 × 50.8mm PCB standard business card size. The antenna takes up most of the right side of the board, with the passive components clustered near the chip on the left. The silkscreen layer on top carries the card's identity name, links, and custom art printed in white over the soldermask. The whole thing is assembled by [JLCPCB](https://jlcpcb.com/) with SMT components, so it arrives ready to program and hand out.

OshWLab Link: https://oshwlab.com/nsreeni2010/project_comtrrqb

<img width="862" height="490" alt="Screenshot 2026-06-25 221014" src="https://github.com/user-attachments/assets/82daf533-5650-48e9-8a02-71568d8244ac" />
<img width="873" height="497" alt="Screenshot 2026-06-25 221406" src="https://github.com/user-attachments/assets/57e9a2c1-6218-4658-8b40-dfa20f411566" />
<img width="1768" height="595" alt="Screenshot 2026-06-25 215907" src="https://github.com/user-attachments/assets/5da4abc1-b17f-4f4a-9ad5-6a366525c50a" />
<img width="976" height="683" alt="Mach Card Schematic" src="https://github.com/user-attachments/assets/a14d0110-8849-45ad-baf4-0bb0abe56356" />

