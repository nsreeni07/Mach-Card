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

|FIELD1|No.   |Quantity  |Comment                    |Designator  |Footprint                                       |Value   |Manufacturer Part            |Manufacturer        |Supplier Part  |Supplier   |Link                                                                                                                                                                                                                                         |
|------|------|----------|---------------------------|------------|------------------------------------------------|--------|-----------------------------|--------------------|---------------|-----------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|      |----: |:--------:|:--------------------------|:-----------|:---------------------------------------------- |:-------|:----------------------------|:-------------------|:--------------|:--------- |------                                                                                                                                                                                                                                       |
|      | 1    | 1        | 220nF                     | C1         | C0603                                          | 220nF  | CL10B224KA8NNNC             | SAMSUNG (三星)       | C21120        | LCSC      |https://www.lcsc.com/product-detail/C1591.html?s_z=n_q_t_C0603&spm=wm.fly.bg.0.xh___wm.ssy.tc.1.tz&lcsc_vid=TlBcBQEAR1AIVgUARllZU1BSEQIIBl1SQQdYBAJUQlgxVlNeQVJfUlBfQVRbUjsOAxUeFF5JWBYZEEoKFBINSQcJGk4%3D                                   |
|      | 2    | 1        | KT-0603B                  | LED1       | LED0603-RD                                     |        | KT-0603B                    | KENTO              | C2288         | LCSC      |https://www.lcsc.com/product-detail/C2288.html?s_z=n_q_KT-0603B%2520%2520%2520&spm=wm.fly.bg.0.xh&lcsc_vid=TlBcBQEAR1AIVgUARllZU1BSEQIIBl1SQQdYBAJUQlgxVlNeQVJfUlFQRFJdXjsOAxUeFF5JWBYZEEoKFBINSQcJGk4dAgUUFAk%3D                            |
|      | 3    | 1        | 47Ω                       | R1         | R0603                                          | 47Ω    | 0603WAF470JT5E              | UNI-ROYAL (厚声)     | C23182        | LCSC      |https://www.lcsc.com/product-detail/C114623.html?s_z=n_q_t_47%25CE%25A9&spm=wm.fly.bg.0.xh___wm.ssy.tc.0.tz&lcsc_vid=TlBcBQEAR1AIVgUARllZU1BSEQIIBl1SQQdYBAJUQlgxVlNeQVJfUlFRT1lbXjsOAxUeFF5JWBYZEEoKFBINSQcJGk4NBhADEA4cHktSRlNADxALGw%3D%3D|
|      | 4    | 1        | NT3H2111W0FHKH            | U1         | XQFN-8_L1.6-W1.6-P0.50-BL_NT3H2111W0FHKH       |        | NT3H2111W0FHKH              | NXP (恩智浦)          | C710403       | LCSC      |https://www.lcsc.com/product-detail/C710403.html?s_z=n_q_NT3H2111W0FHKH&spm=wm.fly.bg.0.xh&lcsc_vid=TlBcBQEAR1AIVgUARllZU1BSEQIIBl1SQQdYBAJUQlgxVlNeQVJfUlFfQFdeUzsOAxUeFF5JWBYZEEoKFBINSQcJGk4eFQsCAgIaSgADAwAHC0slRlRXVkoOAwwC             |
|      | 5    | 1        | 25X48MM_NFC_ANTENNA       | U2         | 25X48MM_NFC_ANTENNA                            |        |                             |                    |               |           |                                                                                                                                                                                                                                             |

