# Harmonic Distortion

<img width="1081" height="791" alt="image" src="https://github.com/user-attachments/assets/271d83f4-81e3-49ae-8bd9-6f1ff293f89f" />

<img width="1074" height="783" alt="image" src="https://github.com/user-attachments/assets/d8e3dd38-f314-42f0-9189-62710b089761" />

<img width="1186" height="350" alt="image" src="https://github.com/user-attachments/assets/ee61a6d0-c77d-426f-a7e1-e717c1b3c576" />

# Why does harmonic distortion happen?

Because real amplifiers are not perfectly linear.
When you increase the input power, the active device (BJT, MOSFET, HEMT) enters:

Nonlinear gm region

Soft compression

Hard clipping

Saturation

As a result, the output waveform gets "bent", creating harmonic components.

# Types of Harmonic Distortion

<img width="1239" height="530" alt="image" src="https://github.com/user-attachments/assets/4c60af52-f641-4f1c-bd5a-1ea944f17658" />

# Why harmonic distortion is important in RF & Microwave?
Because harmonics can:
Interfere with adjacent channels,
Cause spectral regrowth,
Reduce EVM / degrade modulation accuracy,
Harm compliance with FCC/ETSI standards,
Cause receiver blocking,
Reduce power amplifier efficiency due to unwanted outputs,
For LNAs:
→ Low harmonic distortion = better linearity, IMD, IIP3, SFDR

# How to reduce harmonic distortion?
## Increase Linearity of the transistor
1.Use larger transistor
2.Bias at a more linear region ( Class A bias)
3.Increase vgs bias on mosfet/ Vf bias on Bjt
4.Keep gain small signal ( avoid compression)

## Use feedback

1.Resistive feedback reduces distortion
2.But can reduce gain

## Use degeneration

1.Source/emitter degeneration linearizes gm
2.Trade-off: reduces gain/noise

## Improve matching

Proper input/output matching keeps device in linear zone

## Reduce input power

1.Avoid P1dB region
2.Avoid saturation

# Some Important Parameters to know 

## P1dB (1-dB Compression Point)
<img width="1221" height="588" alt="image" src="https://github.com/user-attachments/assets/0899936f-82a8-4ce5-b199-b3590d83e293" />
For More about the 1db Compression Point click on this link - https://www.allaboutcircuits.com/technical-articles/using-the-1-db-compression-point-to-characterize-rf-system-nonlinearity/


## IMD3 (Third-Order Intermodulation Distortion)
<img width="1107" height="519" alt="image" src="https://github.com/user-attachments/assets/7b2f0df1-3c9b-4d11-a488-9bdb88f8c62e" />
<img width="997" height="731" alt="image" src="https://github.com/user-attachments/assets/395d5bb4-b478-4176-9936-4885d9566f94" />

For More about third order intermodultaion distortion click on this  link - https://www.allaboutcircuits.com/technical-articles/understanding-intermodulation-distortion-and-the-third-order-intercept-point-in-rf-systems/

### Why a Single-Tone Harmonic Test Can Be Misleading

<img width="1383" height="271" alt="image" src="https://github.com/user-attachments/assets/e97cccdb-e24c-4236-bab4-4b846928298e" />

<img width="1216" height="529" alt="image" src="https://github.com/user-attachments/assets/efdb103d-114a-4f20-ac48-7e6a175f4e28" />

<img width="1345" height="432" alt="image" src="https://github.com/user-attachments/assets/d0644d76-b3ba-43ad-b00c-ae84e3fb3254" />

<img width="1139" height="479" alt="image" src="https://github.com/user-attachments/assets/417a8225-68d9-4ce9-a2dd-1b99fd65ad1a" />

<img width="1524" height="552" alt="image" src="https://github.com/user-attachments/assets/6ed9d61a-81df-4132-a494-928fae13a48c" />

<img width="1083" height="686" alt="image" src="https://github.com/user-attachments/assets/dec855cc-15a2-4e91-aa85-4e83dc2b7859" />

<img width="1115" height="456" alt="image" src="https://github.com/user-attachments/assets/f7217377-7a04-45c8-af27-619ae66f53ab" />

<img width="1309" height="705" alt="image" src="https://github.com/user-attachments/assets/8f152e9e-570a-4bf2-9bf4-3b6cbdb2db2b" />

<img width="1425" height="362" alt="image" src="https://github.com/user-attachments/assets/2f0ca9dd-9ce2-4479-9c6f-2a9f49775a11" />

<img width="1416" height="518" alt="image" src="https://github.com/user-attachments/assets/802caf37-e89d-4fc1-8ec3-3dd930a170f2" />

# Understanding Dynamic Range and Spurious-Free Dynamic Range in RF Systems

https://www.allaboutcircuits.com/technical-articles/understanding-dynamic-range-and-spurious-free-dynamic-range-in-rf-systems/

## Why Very Low Input Power Is a Problem

<img width="1087" height="333" alt="image" src="https://github.com/user-attachments/assets/b1d1ca71-50c0-428a-8415-d6e929f2c41a" />

## Why Very High Input Power Is a Problem

<img width="1236" height="385" alt="image" src="https://github.com/user-attachments/assets/6bc0211e-4806-4232-a142-0a8ed7e0d8af" />

## Dynamic Range (DR)

<img width="1095" height="328" alt="image" src="https://github.com/user-attachments/assets/da5e8ed7-4aa0-41ef-9af6-5cab9e448c43" />

## Spurious-Free Dynamic Range (SFDR)

<img width="1071" height="343" alt="image" src="https://github.com/user-attachments/assets/c66dfdc5-bfa2-42a7-a5d6-cc7fe10e4459" />

# Power Flow Diagram

         ┌───────────────────────────┐
         │       SOURCE (Vs, Rs)     │
         └─────────────┬─────────────┘
                       │
               Available Input Power
                       │
                       ▼
                P_AS (from source)
                       │
                       │
                       ▼
          ┌───────────────────────────┐
          │   INPUT MATCH NETWORK     │
          └─────────────┬─────────────┘
                       │
               Some power reflected
                       │
                       ▼
                Actual Power Entering
                       │
                       ▼
                P_in (to amplifier)
                       │
                       │
                       ▼
          ┌───────────────────────────┐
          │        AMPLIFIER         │
          └─────────────┬─────────────┘
                       │
              Generates Power
                       │
                       ▼
          Power Available at Output
                       │
                       ▼
                P_Ao (ideal matched)
                       │
                       │
                       ▼
          ┌───────────────────────────┐
          │    OUTPUT MATCH NETWORK   │
          └─────────────┬─────────────┘
                       │
               Some power reflected
                       │
                       ▼
          Power Delivered to Load
                       │
                       ▼
                P_L (actual)


<img width="1023" height="349" alt="image" src="https://github.com/user-attachments/assets/5c56f122-bee6-49fa-b0ec-20ecd9445be5" />



<img width="1198" height="744" alt="image" src="https://github.com/user-attachments/assets/816c67f0-5e38-41e2-a505-877566609b2d" />

<img width="1029" height="264" alt="image" src="https://github.com/user-attachments/assets/6c34910b-4183-4575-983d-8f5eb7c72c91" />

# reducing IM3 (third-order intermodulation) is one of the central practical challenges in RF amplifier/receiver design. Below I give a compact, engineer-friendly guide: the physics, the most effective techniques, the trade-offs, and a short design checklist you can use right away.

<img width="1354" height="689" alt="image" src="https://github.com/user-attachments/assets/c43fcca0-e76d-4f4f-9329-cb1d7a52e8fa" />

<img width="1194" height="678" alt="image" src="https://github.com/user-attachments/assets/d67f4810-3ab1-4407-b432-ff44438e3b2b" />

<img width="1484" height="522" alt="image" src="https://github.com/user-attachments/assets/c0f3841b-795a-4bba-9bd6-2d336fbf430f" />

<img width="1372" height="658" alt="image" src="https://github.com/user-attachments/assets/1e5add78-c716-4f16-8065-006e89c25946" />

<img width="1295" height="464" alt="image" src="https://github.com/user-attachments/assets/8e248303-1b12-4093-ba53-1d1bf3339c24" />

































