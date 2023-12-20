# Overview

This project focuses on DNA sequence compression utilizing a Bayesian approach to optimize the coding of genetic information into binary digits. The provided Python script demonstrates the application of Variable-Length Codes to achieve an efficient representation of DNA sequences in binary format.

The code begins by fetching a DNA sequence from a specified URL, followed by a frequency analysis of the nucleotide occurrences in the sequence. The Bayesian approach is then employed to devise an optimal coding scheme that maps DNA's four-letter alphabet (A, T, C, G) to binary digits. The goal is to achieve compression substantial enough to fit the sequence into memory.

# Bayesian Approach

The Bayesian approach is leveraged to iteratively explore different mappings from DNA letters to binary representations. The effectiveness of each mapping is evaluated based on the resulting compression ratio. The final chosen mapping is applied to convert the DNA sequence into a binary representation.

# Variable-Length Codes

The Variable-Length Codes, specified in the code_opt dictionary, provide an optimum approach to encode the DNA sequence into binary. The lengths of the codes are chosen based on the frequency analysis, allowing more common nucleotides to have shorter binary representations, contributing to compression.

# Statistical Analysis

The script showcases statistical analysis skills by assessing the compression achieved and determining whether the resulting binary representation can be decoded unambiguously back to the original DNA sequence. The analysis considers the size of the compressed data in kilobytes and evaluates whether it meets the threshold for storage on a typical flash drive.

**Note:** The script outputs the compressed binary representation (seq_opt) and verifies the accuracy of decoding. If the compression achieves a size below a specified threshold, it is deemed suitable for storage on a flash drive.

By exploring different coding schemes and leveraging statistical analysis, this project demonstrates an approach to compressing DNA sequences, providing insights into the application of information theory in genomics.
