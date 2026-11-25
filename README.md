# Preprints

November 25, 2026

## [The Complexity of Zero Testing for Three-Factor Geometric Hyperdeterminants](preprints/The-Complexity-of-Zero-Testing-for-Three-Factor-Geometric-Hyperdeterminants-November-25-2026/paper.pdf)

Theorem 1 proves deterministic NP-hardness of geometric hyperdeterminant zero
testing for the formats $(2d-1)\times d\times d$ and $(2d-2)\times d\times d$.
In both families the problem is NP-complete on dense integer tensors with
nonzero symmetric rank-one slices $u_i u_i^{\mathsf T}$ whose factors have
nonnegative integer coordinates. Theorem 2 gives a one-sided randomized
reduction for equal-sided tensors. The paper also gives the split-slice
factorization, counting results, and fixed-characteristic extensions.

Byline and signing fingerprint `82C6 65A0 F85E 0FFA 1735 B4EC C631 F3C6 C291 455A`.

[LaTeX source](preprints/The-Complexity-of-Zero-Testing-for-Three-Factor-Geometric-Hyperdeterminants-November-25-2026/build/Paper.tex) · [Public key](preprints/The-Complexity-of-Zero-Testing-for-Three-Factor-Geometric-Hyperdeterminants-November-25-2026/author-key.asc) · [PDF signature](preprints/The-Complexity-of-Zero-Testing-for-Three-Factor-Geometric-Hyperdeterminants-November-25-2026/paper.pdf.sig.asc)

## [Preimage Reporting with Certified Worst-Case Query Time](preprints/Preimage-Reporting-with-Certified-Worst-Case-Query-Time-November-25-2026/paper.pdf)

The paper gives a static preimage index that reports every preimage within
the collision-sensitive worst-case query bound for every accepted index.
The construction uses isolated walks and stores uncovered inputs explicitly.
It also supports exact counting without enumerating the output.

Byline and signing fingerprint `82C6 65A0 F85E 0FFA 1735 B4EC C631 F3C6 C291 455A`.

[LaTeX source](preprints/Preimage-Reporting-with-Certified-Worst-Case-Query-Time-November-25-2026/build/Paper.tex) · [Public key](preprints/Preimage-Reporting-with-Certified-Worst-Case-Query-Time-November-25-2026/author-key.asc) · [PDF signature](preprints/Preimage-Reporting-with-Certified-Worst-Case-Query-Time-November-25-2026/paper.pdf.sig.asc)

## [From formal Semaev polynomials to the sparse permanent](preprints/From-Formal-Semaev-Polynomials-to-the-Sparse-Permanent-November-25-2026/paper.pdf)

Draft for specialist review.

Byline and signing fingerprint `82C6 65A0 F85E 0FFA 1735 B4EC C631 F3C6 C291 455A`.

The draft shows how a circuit for the full formal Semaev polynomial on a
fixed elliptic curve yields a border circuit for the permanent of a bipartite
graph. The quantitative lower bound uses the sparse-support theorem in the
November 24 permanent preprint.

[LaTeX source](preprints/From-Formal-Semaev-Polynomials-to-the-Sparse-Permanent-November-25-2026/build/Paper.tex) · [Public key](preprints/From-Formal-Semaev-Polynomials-to-the-Sparse-Permanent-November-25-2026/author-key.asc) · [PDF signature](preprints/From-Formal-Semaev-Polynomials-to-the-Sparse-Permanent-November-25-2026/paper.pdf.sig.asc)

## Build

Each paper's `build/` directory contains `Paper.tex` and `style.tex`.
With Tectonic installed, run the following from that directory.

```sh
tectonic Paper.tex
```

The resulting `build/Paper.pdf` is a local build. The detached signatures
apply to the distributed PDFs.

## Verify a PDF signature

With GnuPG installed, run the following from any of the three paper
directories. The temporary keyring keeps verification separate from your
usual keyring.

```sh
verify_dir=$(mktemp -d) &&
gpg --no-options --batch --homedir "$verify_dir" --dearmor \
  --output "$verify_dir/author-key.gpg" author-key.asc &&
gpgv --homedir "$verify_dir" --keyring "$verify_dir/author-key.gpg" \
  --status-fd 1 paper.pdf.sig.asc paper.pdf
```

Check that `VALIDSIG` reports the signing fingerprint listed for the paper.

## Citations

```bibtex
@misc{HyperdeterminantZeroTesting2026,
  author = {{OpenPGP fingerprint 82C6 65A0 F85E 0FFA 1735 B4EC C631 F3C6 C291 455A}},
  title = {{The Complexity of Zero Testing for Three-Factor Geometric Hyperdeterminants}},
  howpublished = {Preprint},
  year = {2026},
  month = nov,
  note = {November 25 edition}
}

@misc{CertifiedPreimageReporting2026,
  author = {{82C6 65A0 F85E 0FFA 1735 B4EC C631 F3C6 C291 455A}},
  title = {{Preimage Reporting with Certified Worst-Case Query Time}},
  howpublished = {Preprint},
  year = {2026},
  month = nov,
  note = {November 25 edition}
}

@misc{FormalSemaevToSparsePermanent2026,
  author = {{82C6 65A0 F85E 0FFA 1735 B4EC C631 F3C6 C291 455A}},
  title = {{From formal Semaev polynomials to the sparse permanent}},
  howpublished = {Preprint},
  year = {2026},
  month = nov,
  note = {November 25 draft for specialist review}
}
```

## License

The manuscripts, their LaTeX sources and styles, and this README are
licensed under [Creative Commons Attribution 4.0 International](LICENSE)
(CC BY 4.0). Use the citations above for attribution details.
