# Distributed Computing - TD

This repository contains modular and reusable teaching materials used to build the exercise booklte for the Distributed Systems course at Nantes University. 
See the [main organization](https://github.com/DistributedComputing/) for more information on the course and additional resources.

## Latest PDFs:
- [TD](https://DistributedComputing.github.io/TD/SCSD.pdf) : compiled version

## Structure

├── LICENSE.md            # License CC-BY-SA 4.0  
├── Makefile              # Automatic compilation  
├── README.md             # This file  
├── build/                # Temporary files used during compilation  
├── latex-libs/           # Dependency from [latex-libs](https://github.com/MatthieuPerrin/latex-libs)  
├── docs/                 # Final PDF files (i.e. compiled booklet)  
├── src/                  # LaTeX source files  
│   ├── drivers/          # Main document files for the course  
│   ├── frame/            # Individual slides organized by topic (one file per slide)  
│   └── img/              # (shareable) images used in the slides  


## Compilation

To build the exercise sheet PDF:

```bash
make
```

This creates `docs/td.pdf`.

Other commands:

```bash
make correction # Builds `docs/correction.pdf`  
make all        # Builds `docs/td.pdf` and `docs/correction.pdf`  
make clean      # Remove temporary files in build/  
make cleanall   # Also remove PDFs in docs/  
```

## Dependencies

These slides rely on styles from the [latex-libs](https://github.com/MatthieuPerrin/latex-libs) project.
- On the first build, the Makefile automatically clones the library into `./latex-libs` (internet required).
- Subsequent builds work offline.
- Update both this repo and the library with:

```bash
make update
```


## Licensing

Content is available under the **Creative Commons Attribution-ShareAlike 4.0 International License** (CC BY-SA 4.0).

This means:
- You are free to reuse, modify, and redistribute the material.
- You must give appropriate credit.
- You must distribute derivatives under the same license.

See [`LICENSE.md`](LICENSE.md) for full terms.

## Contributions

Contributions are welcome!

Each slide is in a separate file, making it easy to reuse or improve specific parts. You can:
- Propose new exercises
- Improve existing content or visuals
- Translate to other languages

Use pull requests to suggest changes.
