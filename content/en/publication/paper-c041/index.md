---
title: "DeXOR: Enabling XOR in Decimal Space for Streaming Lossless Compression of Floating-point Data"
authors:
  - "Chuanyi Lv"
  - "Huan Li"
  - "Dingyu Yang"
  - "Zhongle Xie"
  - "Lu Chen"
  - "Christian S. Jensen"
date: "2025-01-01"
publishDate: "2025-01-01"
publication_types:
  - "paper-conference"
publication: "The 51th International Conference on Very Large Data Bases (VLDB)"
slug: "paper-c041"
abstract: "With streaming floating-point numbers being increasingly preva- Erase lower 32bits Erase lower 39bits Integer part Separate lent, effective and efficient compression of such data is critical. 64-64 Compression schemes must be able to exploit the similarity, or Scale to integer smoothness, of consecutive numbers and must be able to contend with extreme conditions, such as high-precision values or the ab- 39-32=7 erased bits wasted !! Same fraction 0.5 wasted!! sence of smoothness. We present DeXOR, a novel framework that (a) Elf Output Stream (b) Camel Output Stream enables decimal xor procedure to encode decimal-space longest common prefixes and suffixes, achieving optimal prefix reuse and Same exponent found effective redundancy elimination. To ensure accurate and low-cost Decimal XOR Scale 0.06 Exponential subtraction decompression even with binary-decimal conversion errors, DeXOR Exception Handler incorporates 1) scaled truncation with error-tolerant rounding and No similarities wasted. extreme case Redundancies eliminated. 2) different bit management strategies optimized for decimal xor. (c) DeXOR (ours) Output Stream Additionally, a robust exception handler enhances stability by man- aging floating-point exponents, maintaining high compression ra- Figure 1: Compressing the target 64.56 with the previous tios under extreme conditions. In evaluations across 22 datasets, value 64.5487: (a) Elf [30, 32] removes trailing zeros in the bi- DeXOR surpasses state-of-the-art schemes, achieving a 15% higher nary representation but wastes bits after xor. (b) Camel [45] compression ratio and a 20% faster decompression speed while targets the integer part of a decimal value, leaving the frac- maintaining a competitive compression speed. DeXOR also offers tional part unoptimized. (c) DeXOR extracts the longest com- scalability under varying conditions and exhibits robustness in mon decimal prefix (64.5) to exploit smoothness and scales extreme scenarios where other schemes fail. the suffix (from 0.06 to 6) to remove redundancy. It also in- cludes an exception handler based on exponential subtrac- tion for extreme-case target values (127.14716377 · · ·)."
keywords:
  - "dexor"
  - "enabling"
  - "xor"
  - "decimal"
  - "space"
  - "streaming"
  - "lossless"
  - "compression"
doi: "10.14778/3796195.3796200"
links:
  - name: "DBLP"
    url: "https://dblp.org/rec/journals/pvldb/LvLYXCJ26"
  - name: "Project"
    url: "https://longaspire.github.io/publication/"
---
