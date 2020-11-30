## ΑΡΧΙΤΕΚΤΟΝΙΚΗ ΠΡΟΗΓΜΕΝΩΝ ΥΠΟΛΟΓΙΣΤΩΝ

### 2η Εργαστηριακή Άσκηση
#### Design Space Exploration με τον gem5 

**1.** Από τα config.ini αρχεία του κάθε benchmark, βλέπουμε στο Line 15 ότι το μέγεθος της cache line είναι  **cache\_line_size=64**.

**2.** Για το κάθε benchmark, χρησιμοποιούμε το αντίστοιχο αρχείο stats.txt για να αντλήσουμε τις εξής πληροφορίες:

* **BZIP**   
**(i)** Line 12: **sim\_seconds=0.083718** (_χρόνος εκτέλεσης_)   
**(ii)** Line 16: **system.cpu.cpi=1.674353** (_cycles per instruction_)  
**(iii)** 
	* Line 124: **system.cpu.dcache.overall\_miss_rate::total=0.014248** (_συνολικό miss rate για την L1 data cache_)
	* Line 331: **system.cpu.icache.overall\_miss\_rate::total=0.000077** (_συνολικό miss rate για την L1 instruction cache_)   
	* Line 494: **system.l2.overall\_miss_rate::total=0.295243** (_συνολικό miss rate για την L2 cache_)

* **MCF**  
**(i)** Line 12: **sim\_seconds=0.064937** (_χρόνος εκτέλεσης_)   
**(ii)** Line 16: **system.cpu.cpi=1.298734** (_cycles per instruction_)  
**(iii)** 
	* Line 124: **system.cpu.dcache.overall\_miss_rate::total=0.002079** (_συνολικό miss rate για την L1 data cache_)
	* Line 332: **system.cpu.icache.overall\_miss\_rate::total=0.023610** (_συνολικό miss rate για την L1 instruction cache_)   
	* Line 496: **system.l2.overall\_miss_rate::total=0.055082** (_συνολικό miss rate για την L2 cache_)

* **HMMER**   
**(i)** Line 12: **sim\_seconds=0.059390** (_χρόνος εκτέλεσης_)   
**(ii)** Line 16: **system.cpu.cpi=1.187803** (_cycles per instruction_)  
**(iii)** 
	* Line 124: **system.cpu.dcache.overall\_miss_rate::total=0.001628** (_συνολικό miss rate για την L1 data cache_)
	* Line 348: **system.cpu.icache.overall\_miss_rate::total=0.000212** (_συνολικό miss rate για την L1 instruction cache_)   
	* Line 512: **system.l2.overall\_miss_rate::total=0.078296** (_συνολικό miss rate για την L2 cache_)

* **SJENG**   
**(i)** Line 12: **sim\_seconds=0.513811** (_χρόνος εκτέλεσης_)   
**(ii)** Line 16: **system.cpu.cpi=10.276223** (_cycles per instruction_)  
**(iii)** 
	* Line 124: **system.cpu.dcache.overall\_miss_rate::total=0.121831** (_συνολικό miss rate για την L1 data cache_)
	* Line 329: **system.cpu.icache.overall\_miss\_rate::total=0.000020** (_συνολικό miss rate για την L1 instruction cache_)   
	* Line 491: **system.l2.overall\_miss_rate::total=0.999972** (_συνολικό miss rate για την L2 cache_)

* **LIBM**   
**(i)** Line 12: **sim\_seconds=0.174771** (_χρόνος εκτέλεσης_)   
**(ii)** Line 16: **system.cpu.cpi=3.495428** (_cycles per instruction_)  
**(iii)** 
	* Line 124: **system.cpu.dcache.overall\_miss_rate::total=0.060972** (_συνολικό miss rate για την L1 data cache_)
	* Line 331: **system.cpu.icache.overall\_miss\_rate::total=0.000093** (_συνολικό miss rate για την L1 instruction cache_)   
	* Line 493: **system.l2.overall\_miss_rate::total=0.999944** (_συνολικό miss rate για την L2 cache_)





