---
title: "DeXOR: Enabling XOR in Decimal Space for Streaming Lossless Compression of Floating-point Data"
authors:
  - "Chuanyi Lv"
  - "Huan Li"
  - "Dingyu Yang"
  - "Zhongle Xie"
  - "Lu Chen"
  - "Christian S. Jensen"
author_links:
  - name: "Chuanyi Lv"
    url: "/authors/chuanyi-lv/home/"
  - name: "Huan Li"
    url: "/authors/huan-li/home/"
date: "2025-01-01"
publishDate: "2025-01-01"
publication_types:
  - "paper-conference"
publication: "The 51th International Conference on Very Large Data Bases (VLDB)"
venue: "The 51th International Conference on Very Large Data Bases (VLDB)"
publication_kind: "conference"
slug: "paper-c041"
design:
  css_class: single-language-section
venue_rankings:
  - "CCF-A"
  - "CORE-A*"
abstract: "With streaming floating-point numbers being increasingly prevalent, effective and efficient compression of such data is critical. Compression schemes must be able to exploit the similarity, or smoothness, of consecutive numbers and must be able to contend with extreme conditions, such as high-precision values or the absence of smoothness. We present DeXOR, a novel framework that enables decimal xor procedure to encode decimal-space longest common prefixes and suffixes, achieving optimal prefix reuse and effective redundancy elimination. To ensure accurate and low-cost decompression even with binary-decimal conversion errors, DeXOR incorporates 1) scaled truncation with error-tolerant rounding and 2) different bit management strategies optimized for decimal xor. Additionally, a robust exception handler enhances stability by managing floating-point exponents, maintaining high compression ratios under extreme conditions. In evaluations across 22 datasets, DeXOR surpasses state-of-the-art schemes, achieving a 15% higher compression ratio and a 20% faster decompression speed while maintaining a competitive compression speed. DeXOR also offers scalability under varying conditions and exhibits robustness in extreme scenarios where other schemes fail."
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
