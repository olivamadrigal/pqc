# pqc
post-quantum cryptography

NIST PQC Round 3 selected Finalists should have been published by end of March 2022.

Selected candidates will probably be McEliece & Saber for KEMs and Dilithium as DS.

McEliece is the backed 40+ yrs candidate and from the Lattice-based schemes (Saber, Kyber, and NTRU),
Saber based on Module Learning with Rounding is the most promising with respect to simpllicity, security, efficiency,
and practicality. Past schemes based on NTRU have all been broken because one thing or another is overlooked.
Moreover, even within the community, there is confusion regarding non-asymptotic behaviour for new algorithms based on
SVP.

Non-selected finalists and alternates will probably pass on to Round 4 for further studies since cryptanalysis for Rainbow and GeMSS raised concerns at Round 3 stage and Rainbow was broken on "a weekend on a laptop" for catergory I parameters... "Reminder to not put candidates into products UNTIL the standard is done". In accords with Dan Bobeh crypto 101 from many years back, "never use your own crypto"; We have seen how companies have gotten burnt doing that. And even standards get broken eventually, like DES and SHA-1, etc.

https://csrc.nist.gov/CSRC/media/Presentations/status-update-on-the-3rd-round/images-media/session-1-moody-nist-round-3-update.pdf

https://www.youtube.com/watch?v=DcwupScEaOQ

Dilithum with SUF-CMA and varying levels of security (2, 3, & 5) is likely to get selected over Falcon based on simplicity, practicality, and limitations. Falcon for example is a bit more involved and places some constraints, such as 53-bit precision floating point arithmetic... embedded, IoT. 

Besides that, all finalists share common underlying constructus: finite fields, rings, linear algebra, distributions (error distributions), incorporation of existing modern symmetric key crypto (AES) and crypto hash functions and PRNGs. 
