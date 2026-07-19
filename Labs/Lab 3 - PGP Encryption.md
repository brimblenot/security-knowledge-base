---
title: Lab 3 - PGP Encryption
date: 
tags: [lab, cryptography, encryption]
tools: [PGP]
domain: 1 - General Security Concepts
course: CIS 425 (Team 4)
---

# Lab 3 — PGP Software

## Objective
Understand how Pretty Good Privacy (PGP) provides confidentiality, integrity, and authenticity, and demonstrate its use for secure communication.

## Environment / Setup
- Course: CIS 425 (group lab, Team 4)
- Artifacts: `Lab 3 PGP Software.docx`

## Background
PGP is encryption software providing cryptographic privacy and authentication. It uses a **hybrid of symmetric and asymmetric cryptography** to encrypt/decrypt data and **digitally signs** messages so recipients can verify the sender. End-to-end encryption keeps data private. Commonly used for email, but also secures text messages, files, and offline/cold storage.

PGP delivers the CIA triad:
- **Confidentiality** — via encryption
- **Integrity** — digital signatures detect unauthorized changes
- **Authenticity** — signatures verify the sender's identity

## Use-case examples
- **Journalist ↔ whistleblower:** whistleblower encrypts the email + attachments; journalist decrypts with their private key. Ensures only the intended recipient reads it and the message is unaltered.
- **Executive → board:** executive applies a digital signature to financial updates to confirm origin and prove the message wasn't altered in transit.

## What I Learned
PGP's hybrid model is the key insight: asymmetric crypto solves key exchange, symmetric crypto does the bulk encryption efficiently, and digital signatures add integrity + authenticity. This is the same pattern behind TLS — a great anchor for understanding real-world crypto.

## Related
- Sec+ domain 1: PKI, symmetric vs asymmetric, hashing, digital signatures
- Concept: hybrid encryption / key exchange
