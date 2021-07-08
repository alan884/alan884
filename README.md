- 👋 Hi, I’m @alan884
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
alan884/alan884 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
875378// Use eth_RequestAccounts
ethereum.send('eth_requestAccounts').then((accounts: string[]) => {
  console.log(`User's address is ${accounts[0]}`)

  // Optionally, have the default account set for web3.js
  web3.eth.defaultAccount = accounts[0]
})

// Alternatively, you can use ethereum.enable()
ethereum.enable().then((accounts: string[]) => {
  console.log(`User's address is ${accounts[0]}`)
  web3.eth.defaultAccount = accounts[0]
})
