# Arithmetic-operation-using-8086
# 8086 Assembly Language Programs for Arithmetic Operations

## AIM

To write and execute Assembly Language Programs to perform arithmetic operations for the 8086 microprocessor.

---

## APPARATUS REQUIRED

* Personal Computer with MASM Software

---

## 1. ADDITION

#### Algorithm

1. Initialize memory location in HL register.
2. Store 1st data.
3. Increment HL to enter 2nd data.
4. Move 2nd number to accumulator.
5. Decrement HL.
6. Add value in memory with accumulator.
7. Store result.
8. Stop.


## FLOW CHART
<img width="707" height="1024" alt="image" src="https://github.com/user-attachments/assets/b5a7062d-e294-47cd-9683-a40de25e82de" />


#### Program

```
CODE SEGMENT
ASSUME CS:CODE, DS:CODE
ORG 1000H
MOV CL,00H
MOV AX,1234H
MOV BX,1234H
ADD AX,BX
JNC L1
INC CL
L1:MOV SI,1200H
MOV [SI],AX
MOV [SI+2],CL
MOV AH,4CH
INT 21H
CODE ENDS
END

```

#### Output Table

<img width="991" height="405" alt="image" src="https://github.com/user-attachments/assets/4a335a2e-09b8-402f-89d8-8c17efd0b445" />


#### Manual Calculations
<img width="923" height="311" alt="image" src="https://github.com/user-attachments/assets/911e29bc-d9aa-45aa-b952-f493b72eaa59" />

---

## OUTPUT IMAGE FROM MASM SOFTWARE
<img width="826" height="550" alt="image" src="https://github.com/user-attachments/assets/fa0ae106-aede-4cad-934f-d51b31823fca" />


## 2. SUBTRACTION

#### Algorithm

1. Initialize memory and store 1st data.
2. Increment to get 2nd data.
3. Move 2nd data to accumulator.
4. Subtract memory content.
5. Store result.

## FLOWCHART

<img width="578" height="797" alt="image" src="https://github.com/user-attachments/assets/564c3c7a-33ce-4a1c-8920-beb5c24b9b47" />


#### Program
```code segment
assume cs:code,ds:code
org 1000h
mov AX,1234h
mov BX,1234h
sub AX,BX
jnc down
inc CL
down:mov SI,1200h
mov [sI],AX
mov [SI+2],CL
mov ah,4ch
int 21H
code ends
end

```


#### Output Table
<img width="1010" height="413" alt="image" src="https://github.com/user-attachments/assets/9e771cd7-ae64-42ca-8809-84f6e9d9632f" />



#### Manual Calculations

<img width="606" height="374" alt="image" src="https://github.com/user-attachments/assets/80d93ea7-4f5a-44d7-ab05-24d8710ecce1" />

---


## OUTPUT SCREEN FROM MASM SOFTWARE
<img width="818" height="545" alt="image" src="https://github.com/user-attachments/assets/0a37e052-9c91-480f-afaf-cf3359469c9e" />

## 3. MULTIPLICATION

#### Algorithm

1. Initialize memory and store operands.
2. Move operands to registers.
3. Multiply.
4. Store result.

##FLOWCHART

<img width="569" height="906" alt="image" src="https://github.com/user-attachments/assets/88be88ff-2896-4a88-b73d-84ccffd2fcf9" />



#### Program

```
code segment
assume cs:code,ds:code
org 1000h
MOV DX,0000H
mov AX,1234h
mov BX,1234h
mul BX
mov si,1200h
mov [si],ax
mov [si+02h],dx
mov ah,4ch
int 21h
code ends
end

```

#### Output Table

<img width="940" height="632" alt="image" src="https://github.com/user-attachments/assets/e9ffc18e-dc7c-49dc-8125-5b3e0dec1351" />


#### Manual Calculations

<img width="683" height="568" alt="image" src="https://github.com/user-attachments/assets/91ee4c25-0d19-40de-8b68-02e85a0215d3" />


---

## OUTPUT SCREEN FROM MASM SOFTWARE
<img width="992" height="478" alt="image" src="https://github.com/user-attachments/assets/86dcdd98-c116-4157-9e95-d45263175393" />


## 4. DIVISION

#### Algorithm

1. Load memory location of operands.
2. Perform division.
3. Store result.

   ## FLOWCHART
<img width="1065" height="802" alt="image" src="https://github.com/user-attachments/assets/25b4a483-0d42-494b-8639-1af3ea17191b" />


#### Program

```
CODE SEGMENT
ASSUME CS:CODE,DS:CODE
ORG 1000H
MOV DX,0000H
MOV AX,1234H
MOV BX,1234H
DIV BX
MOV SI,1200H
MOV [SI],AX
MOV [SI+02H],DX
MOV AH,4CH
INT 21H
CODE ENDS
END

```

#### Output Table

<img width="940" height="609" alt="image" src="https://github.com/user-attachments/assets/565b717d-add8-4ce0-aba4-7621bc27ae32" />


#### Manual Calculations

<img width="520" height="421" alt="image" src="https://github.com/user-attachments/assets/bd03a483-3b28-4a8e-a8d1-6c05ed2dfb1f" />

---
## OUTPUT FROM MASM SOFTWARE

<img width="940" height="629" alt="image" src="https://github.com/user-attachments/assets/d6d93ed3-8849-4f60-8897-ccd14fcd079a" />


## RESULT

Thus, the Assembly Language Programs for 8086 to perform arithmetic operations (Addition, Subtraction, Multiplication, and Division) using both direct and indirect methods were successfully written and executed using MASM.

