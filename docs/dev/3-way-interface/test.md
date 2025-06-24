flowchart TD
    A_AUX_out(A AUX out)
    B_AUX_in>B AUX in]
    A_PTT_out(A PTT out)
    B_PTT_in>B PTT in]
    B_AUX_out(B AUX out)
    A_AUX_in>A AUX in]
    B_PTT_out(B PTT out) 
    A_PTT_in>A PTT in]
    A_GND
    B_GND

    %% Direct Pinout
    A_GND    --> B_GND
    A_AUX_out --> B_AUX_in
    A_PTT_out --> B_PTT_in
    B_AUX_out --> A_AUX_in
    B_PTT_out --> A_PTT_in
    
    %% %% From radio to pc
    %% A_AUX_out --> R1
    %% R1 --> PC_AUX_in
    %% A_PTT_out --> |control | R1

    %% B_AUX_out --> R2
    %% B_PTT_out --> |control | R2
    %% R2 --> PC_AUX_in

    %% %% From PC to radio
    %% PC_AUX_out --> A_AUX_in
    %% PC_AUX_out --> B_AUX_in

    %% PC_PTT_out -->|control| R3
    %% R3 --> A_PTT_in

    %% PC_PTT_out -->|control| R4
    %% R4 --> B_PTT_in




