#### Notes for lab 1

* Misc
  * `static` variable in function is not store in stack, cannot corrupt activation record

* [Buffer Overflows: Attacks and Defenses for the Vulnerability of the Decade](http://css.csail.mit.edu/6.858/2014/readings/buffer-overflows.pdf)
  * Stack Guard, Stack Canary
  * Type:
  	1. Corrupt activation record(ret for function call) (stack smashing)
  	2. Corrupt function pointer
  	3. Corrupt buffer in [`longjump(buffer)`](http://en.cppreference.com/w/cpp/utility/program/longjmp)
  * Check `strcpy` and `sprintf`
  