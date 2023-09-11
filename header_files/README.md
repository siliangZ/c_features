# The include order
1. header files corresponding to the source file
2. header files from the same component/project
3. header files from other components/projects
4. system header files(standard c headers)

## Rationale
1. each header file should be self-contained.(no prerequisistes)


Quote from <<Thinking in C++>>
> Latent usage errors can be avoided by ensuring that the .h file of a component parses by itself – without externally-provided declarations or definitions... Including the .h file as the very first line of the .c file ensures that no critical piece of information intrinsic to the physical interface of the component is missing from the .h file (or, if there is, that you will find out about it as soon as you try to compile the .c file).
