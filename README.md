<!-- Don't delete it -->
<div name="readme-top"></div>

<!-- Organization Logo -->
<div align="center" style="display: flex; align-items: center; justify-content: center; gap: 16px;">
  <img alt="Stability Nexus" src="public/stability.svg" width="175">
  <img src="public/todo-project-logo.svg" width="175" />
</div>

&nbsp;

<!-- Organization Name -->
<div align="center">

[![Static Badge](https://img.shields.io/badge/Stability_Nexus-HodlCoin_Phoenix-228B22?style=for-the-badge&labelColor=FFC517)](https://stability.nexus/)

</div>

<p align="center">
<!-- Telegram -->
<a href="https://t.me/StabilityNexus">
<img src="https://img.shields.io/badge/Telegram-black?style=flat&logo=telegram&logoColor=white&color=24A1DE"/></a>
&nbsp;&nbsp;
<!-- X -->
<a href="https://x.com/StabilityNexus">
<img src="https://img.shields.io/twitter/follow/StabilityNexus"/></a>
&nbsp;&nbsp;
<!-- Discord -->
<a href="https://discord.gg/YzDKeEfWtS">
<img src="https://img.shields.io/discord/995968619034984528?style=flat&logo=discord&logoColor=white&label=Discord&labelColor=5865F2&color=57F287"/></a>
&nbsp;&nbsp;
<!-- Medium -->
<a href="https://news.stability.nexus/">
<img src="https://img.shields.io/badge/Medium-black?style=flat&logo=medium&color=white"/></a>
&nbsp;&nbsp;
<!-- LinkedIn -->
<a href="https://linkedin.com/company/stability-nexus">
<img src="https://img.shields.io/badge/LinkedIn-black?style=flat&logo=LinkedIn&color=0A66C2"/></a>
&nbsp;&nbsp;
<!-- YouTube -->
<a href="https://www.youtube.com/@StabilityNexus">
<img src="https://img.shields.io/youtube/channel/subscribers/UCZOG4YhFQdlGaLugr_e5BKw?style=flat&logo=youtube&labelColor=FF0000&color=FF0000"/></a>
</p>

---

<div align="center">
<h1>HodlCoin Phoenix – ErgoScript Contracts</h1>
</div>

The **HodlCoin Phoenix** project contains the ErgoScript smart contracts that implement the Phoenix version of the HodlCoin protocol.  
This repository includes fee-handling rules, token-based implementations, and formal references derived from the HodlCoin research paper.

---


## 📦 Implementation Types

This repository includes two implementations:

1. **[hodlERG](/hodlERG/README.md)** — implementation using ERG.  
2. **[hodlToken](/hodlToken/README.md)** — token-based implementation.

Both follow the HodlCoin Phoenix contract architecture.

---

## 💸 Fee Contract Implementation Guidelines

All HodlCoin Phoenix fee contract implementations **must** send a minimum fee amount to **Dr. Bruno Woltzenlogel Paleo’s Ergo address**:

9gnBtmSRBMaNTkLQUABoAqmU2wzn27hgqVvezAC9SU1VqFKZCp8

markdown
Copy code

Fee rule:

- Let **Q** = amount paid to Bruno’s address.  
- Let **F** = bank fee percentage.  
- Let **D** = developer fee percentage.  
- Then:

Q ≥ 0.025 × (F / D)

yaml
Copy code

As long as this condition is satisfied, any further custom constraints may be added to the fee contract implementation.

---

## 🧠 References

The HodlCoin protocol is described in the official research paper:

📄 **HodlCoin: A Trustless Savings Protocol for Stable Value Creation**  
https://eprint.iacr.org/2023/1029

---

## 🤝 Contributing

Contributions are welcome!

1. Fork the repo and create a branch (`git checkout -b feature/MyChange`).  
2. Implement changes and write tests if applicable.  
3. Submit a PR with clear explanations.  

For bugs or questions, open an issue with steps to reproduce and logs.

---

© 2025 The Stable Order
