Run the following command to see the first 16 colours of the palette:

```bash
for i in {0..15}; do printf "\x1b[48;5;${i}m %3d \x1b[0m " $i ; if ! (( ($i + 1 ) % 8 )); then echo ; fi ; done
```
