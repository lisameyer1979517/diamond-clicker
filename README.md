# diamond-clicker

## Project Description

**diamond-clicker** is an on-chain clicker game built on the Aptos blockchain. Players earn and upgrade virtual diamonds by interacting with smart contracts, competing for rewards based on their click activity. The project demonstrates gamification mechanics using decentralized ledger technologies.

## Features

- 💎 On-chain click-to-earn gameplay
- 🔥 Upgrade system to boost diamond production
- 🛡️ Secure Move smart contract architecture
- 🏆 Leaderboards and reward distribution mechanisms
- 📈 Designed for scalability and low-cost transactions

## Installation

```bash
# Clone the repository
git clone https://github.com/lisameyer1979517/diamond-clicker.git
cd diamond-clicker

# Install frontend dependencies (if any)
npm install
# or
yarn install
```

## Usage

### Deploy Smart Contracts

```bash
# Compile Move smart contracts
aptos move compile --package-dir move/

# Publish contracts to the Aptos network
aptos move publish --package-dir move/ --profile default
```

### Play the Game

- **Click**: Call the `click` function to increment your diamond count.
- **Upgrade**: Spend diamonds to buy upgrades that generate passive income.
- **Compete**: View leaderboards and compete for the highest score.

Example using Aptos CLI:

```bash
# Make a click
aptos move run-entry-function \
  --function-id "diamond_clicker::game::click" \
  --args "0xYourAddress"
```

### Testing

```bash
# Run Move unit tests
aptos move test --package-dir move/
```

## Configuration

- Adjust parameters such as diamond production rate, upgrade costs, and reward distribution directly in the Move modules.
- Update network settings in `aptos.yaml` for deployment to devnet, testnet, or mainnet.

## Contributing

We welcome community contributions!

1. Fork the repository
2. Create a new branch (`git checkout -b feature/your-feature-name`)
3. Implement your changes
4. Commit your work (`git commit -m 'Add your message here'`)
5. Push to your branch (`git push origin feature/your-feature-name`)
6. Open a pull request

Please refer to [CONTRIBUTING.md](CONTRIBUTING.md) for detailed contribution guidelines.

## License

This project is licensed under the [Apache 2.0 License](LICENSE).

## Links

- [Aptos Documentation](https://aptos.dev/)
- [Move Language Documentation](https://move-language.github.io/move/)
- [Aptos GitHub](https://github.com/aptos-labs)
