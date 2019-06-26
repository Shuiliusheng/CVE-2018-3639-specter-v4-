# CVE-2018-3639-specter-v4
**spectre v4 : Speculative Store Bypass (CVE-2018-3639) proof of concept for Linux**

- **build:** gcc spectre-v4.cpp -o spectre

- **run:** ./spectre


- **result:**

  --------attack--------

  low than threshold:155

  low than threshold:144

  low than threshold:133

  low than threshold:0

  low than threshold:1

  --------attack--------

  low than threshold:133

  low than threshold:0

  low than threshold:1

  --------attack--------

  low than threshold:0

  low than threshold:1


- 
  **Question:**

  every time I want use the same victim function to get other secret data, it will be failed.

  I guess it is because the two  instruction will be marked dependent load and store, so it won't speculate the load instruction.