# program-list-spesifikasi-leptop-lenovo

.model SMALL
.code
ORG 100h

menu:
    jmp mulai1
    l1 db 'list leptop Lenovo : $'
    l2 db 13,10, '[1] Yoga Book 9i $'
    l3 db 13,10, '[2] Yoga 7 $'
    l4 db 13,10, '[3] Yoga 6 $'
    l5 db 13,10, '[0] Keluar $'
    l6 db 13,10, 'Masukkan pilihan anda : $'
    
    entr db 13,10, '$' 
    
    y91 db 13,10,'Prosesor  : Intel Core™ Ultra 7 155U $'
    y92 db 13,10,'Grafis    : Inte Graphics $'
    y93 db 13,10,'RAM       : 32 GB Soldered LPDDR5x-7476 $'
    y94 db 13,10,'ROM       : 1TB SSD M.2 2242 PCIe 4.0×4 NVMe $'
    
    y71 db 13,10,'Prosesor  : Intel Core i5-1135G7 $'
    y72 db 13,10,'Grafis    : Integrated Intel Iris Xe Graphics $'
    y73 db 13,10,'RAM       : 8GB Soldered DDR4-3200 $'
    y74 db 13,10,'ROM       : 512GB SSD M.2 2242 PCIe 3.0x4 NVMe $'
    
    y61 db 13,10,'Prosesor  : AMD Ryzen™ 7 7730U $'
    y62 db 13,10,'Grafis    : Integrated AMD Radeon Graphics $'
    y63 db 13,10,'RAM       : 16GB Soldered LPDDR4x-4266 $'
    y64 db 13,10,'ROM       : 512GB SSD  $'
    
    keluar db 13,10,'Program Selesai! $'
    
    pilih db 23,?,23 dup(?)
    
mulai1:
    mov ah,09h
    lea dx,l1
    int 21h
    lea dx,l2
    int 21h
    lea dx,l3
    int 21h
    lea dx,l4
    int 21h
    lea dx,l5
    int 21h
    lea dx,l6
    int 21h
    mov ah,0ah
    lea dx,pilih 
    int 21h
    
menu1:
    mov ah,09h
    lea dx,entr
    int 21h ;efwqegrnr
    lea dx,l2
    int 21h
    lea dx,y91
    int 21h
    lea dx,y92
    int 21h
    lea dx,y93
    int 21h
    lea dx,y94
    int 21h
    lea dx,entr
    int 21h
        
    mov ah,09h
    lea dx, entr
    int 21h
    lea dx,l1
    int 21h
    lea dx,l2
    int 21h
    lea dx,l3
    int 21h
    lea dx,l4
    int 21h
    lea dx,l5
    int 21h
    lea dx,l6
    int 21h
    mov ah,0ah
    lea dx,pilih 
    int 21h
    
menu2:
    mov ah,09h
    lea dx, entr
    int 21h
    lea dx,l3
    int 21h
    lea dx,y71
    int 21h
    lea dx,y72
    int 21h
    lea dx,y73
    int 21h
    lea dx,y74
    int 21h
    lea dx,entr
    int 21h
    
    mov ah,09h
    lea dx, entr
    int 21h
    lea dx,l1
    int 21h
    lea dx,l2
    int 21h;evdfbg
    lea dx,l3
    int 21h
    lea dx,l4
    int 21h
    lea dx,l5
    int 21h
    lea dx,l6
    int 21h
    mov ah,0ah
    lea dx,pilih 
    int 21h
    
    
menu3:
    mov ah,09h
    lea dx, entr
    int 21h
    lea dx,entr
    int 21h
    lea dx,l4
    int 21h
    lea dx,y61
    int 21h
    lea dx,y62
    int 21h
    lea dx,y63
    int 21h
    lea dx,y64
    int 21h
    lea dx,entr
    int 21h
    
    mov ah,09h
    lea dx,l1
    int 21h
    lea dx,l2
    int 21h
    lea dx,l3
    int 21h
    lea dx,l4
    int 21h
    lea dx,l5
    int 21h
    lea dx,l6
    int 21h
    mov ah,0ah
    lea dx,pilih 
    int 21h
      
    
selesai:
    mov ah,09h
    lea dx, entr
    int 21h
    lea dx,keluar
    int 21h  ;fegrhww
    int 20h
    
END
