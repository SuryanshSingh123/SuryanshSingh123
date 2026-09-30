```asm
[org 0x7c00]

xor ax, ax
mov ds, ax
mov es, ax

mov bp, 0x9000
mov sp, bp

mov ah, 0x0e
mov al, 'H'
int 0x10

hlt ; save your CPU
jmp $

times 510-($-$$) db 0
dw 0xaa55
```

C is very fast.

The best language that AI can write isn't Python or Typescript, it's English.

Currently learning bootloader and kernel development.
May continue to RISC-V and ARM after x86.
