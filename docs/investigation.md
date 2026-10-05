# Cryptography & Data Protection Fundamentals — Investigation Notes

## Objective and evidence

Practice basic confidentiality and integrity concepts. The source consists of three screenshot pages: command-line file operations and binary display; Word document encryption and an AES utility; and AES/hash demonstrations.

## Activities and interpretation

| Activity | Source observation | What it demonstrates |
| --- | --- | --- |
| Document protection | Word Protect Document menu and password-open prompt | Applying password-based document access protection |
| AES demonstration | Utility labeled AES-128; encrypted sample text shown | Symmetric encryption and recovery of plaintext in a teaching tool |
| Hash demonstration | MD5 selected; digest shown for sample text | Fixed-length one-way digest calculation |
| File-based information hiding | Binary copy/file-combination command and binary output | Appending/combining data; not proof of robust steganography |

The document-password prompt contains a personal file path and is not republished. The demonstration key field in the published AES image is masked. Only sample input and the interface are shown.

## Concepts learned

Encryption transforms data with a key so an authorized holder can recover plaintext. A hash produces a digest used in comparisons; it cannot be decrypted to recover the original text. Hiding appended data in a file does not provide the guarantees of encryption. The source MD5 demonstration is a teaching example and is not presented as a modern secure choice for collision-sensitive integrity or password storage.

The original screenshots do not document an authenticated-encryption mode, key derivation, strong key generation, recovery procedures, or tamper detection. Merely using an interface labeled AES-128 does not prove a secure application design.

## Practical lessons

Use synthetic data for browser-based cryptography demonstrations. Real confidential documents, passwords, and keys require trusted local tooling and deliberate key management. A file that still opens after appended data is not evidence that the additional data is hidden from forensic inspection.

## Limitations

No actual encrypted document, source script, original combined image, or round-trip automated test is included. This repository documents foundational coursework and screenshots rather than a deployed security product. Claims of algorithm strength or tool security were not tested in the exercise.
