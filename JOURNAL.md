# ⌨️ SR-U2764 - Journey Log
This is the start of my journey of building my first ever hardware project + pcb + physical thing! i've never been into electronics before, but as soon as i got to know about highway, i quickly decided what i want to build -- my own mechanical keyboard! as keyboards are very expensive, and im planning to build my own desk setup soon, so it will look cool that i have my own made keyboard on my setup.

I want to make it clean, compact, and functional keyboard with no actual flaws. **But doing mistakes is a part of journey - isn't it?**

# 11/07/25
# *Chapter 1️⃣: Deciding Name*
This was the start of this journey - i had to decide a name for this keyboard, at first i thought that i should name it with my surname - Ghalib. something like Ghalib-1.0 or something else, but then i thought it would feel a little bit cringe. then i decided that i want to dedicate it to a special person. Can't name them here - but if you are in my really short list of close friends, you already know that.

So I named this keyboard as codename of the bond between us. You can crack it easily btw 🥲 was'nt able to name something that is easier to understand as well as difficult to crack, but still, i love this one.

# _Chapter 2️⃣: Planning The Specifications_

After that i started thinking about what do i want in this keyboard. It should have enough features as a normal keyboard while also easier to build and design as i have to do everything myself 🥲🥲. So I went for these specifications:

- **60% ANSII Keyboard Layout**
- **Cherry MX Blue Switches**
- **An Oled Panel (Controllable from OS)**
- **Per -Key RGB Lighting**

# 12/07/25

# _Chapter 3️⃣: Finding The Right Components_
I started googling for random keyboard stuff and read some blogs about mechanical keyboards and did'nt understand anything at all, then i randomly added a message in the #highway channel on slack of HackClub. Nofreedom (A really nice guy from HackClub) showed me his Keyboard. It was a life saver, i saw his schematic and it gave me a bit understanding of how to do this stuff. 

I just decided that i'll go for same components as Nofreedom - Only addition will be an OLED Display

Here's The Components I Decided to Use:
- **Raspberry Pi Pico (U2 TFT)**
- **SSD1306-128x64 OLED Display**
- **And CherryMx SW_Push Keys**
- **1N4148 Diodes**

# _Chapter 4️⃣: Designing the Schematic and PCB_

After that at first i just copied and pasted his schematic (I know it's cheating but wait - read more.). Soon I realized that as long as i dont design my own thing, i wont be able to understand and it is crucial to understand the logic of schematic to wire up the PCB. Nofreedom's pcb was good, but his case did'nt look good enough to me. So i Decided to redesign the key matrix. This time it was much easier coz i was constantly playing around with things on Nofreedom's Freeboard.

I redesigned with a 8x10 Matrix grid and connected them to Pico. 

**Designing The PCB**
Then i moved on to the PCB part. I saw a tutorial on youtube which included taking the json from keyboard Layout editor and a plugin (KLMTOKICAD) which would automatically adjust the keys based on the layout. I replicated the process and it was good to go. Now when i opened the 3d viewer in pcb, it had an issue, there was no place to add the oled display as i was using 60% layout and it was packed up with keys. So i decided i also have to add arrow keys, the top area can be then used to add the OLED and a place to add the microcontroller on.

**Routing**
This was the toughest part, it felt like im playing game. while i have no idea if it will work or not, i just cinnected all wires together, and i used a lots of via pads and i dont even know if its normal or not 🙂
 But Atleast it's complete now. I ran all the tests and they are okay