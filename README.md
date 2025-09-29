# MediBlock

## Project Description

MediBlock is a decentralized medical records management system built on blockchain technology. It provides a secure, transparent, and patient-centric approach to storing and managing medical records. The smart contract enables patients to have full control over their medical data while allowing authorized healthcare providers to access and update records with patient consent.

The system ensures data integrity, privacy, and accessibility through blockchain's immutable ledger, eliminating the need for centralized databases that are vulnerable to breaches and unauthorized access.

## Project Vision

Our vision is to revolutionize healthcare data management by:

- **Empowering Patients**: Giving patients complete ownership and control over their medical records
- **Enhancing Security**: Leveraging blockchain's cryptographic security to protect sensitive health information
- **Improving Interoperability**: Creating a standardized system that allows seamless data sharing across healthcare providers
- **Ensuring Transparency**: Maintaining an immutable audit trail of all record access and modifications
- **Reducing Costs**: Eliminating redundant tests and administrative overhead through unified record systems

MediBlock aims to create a future where medical records are portable, secure, and accessible to authorized parties anywhere in the world, while maintaining patient privacy and data sovereignty.

## Key Features

### 1. **Patient Registration**
- Self-registration system for patients
- Patients maintain complete ownership of their data
- Unique blockchain address serves as patient identifier

### 2. **Doctor Verification**
- Admin-controlled doctor verification process
- Ensures only qualified healthcare providers can create records
- Tracks doctor specializations and credentials

### 3. **Medical Record Creation**
- Authorized doctors can create comprehensive medical records
- Records include diagnosis, treatment, timestamps, and doctor information
- Immutable storage ensures record integrity

### 4. **Access Control Management**
- Patients can authorize specific doctors to access their records
- Granular permission system for enhanced privacy
- Ability to revoke access at any time

### 5. **Record Retrieval**
- Patients can view all their medical records
- Authorized doctors can access patient records with consent
- Admin oversight for system management

### 6. **Transparency and Auditability**
- All actions are logged through blockchain events
- Complete audit trail of record creation and access
- Immutable history prevents data tampering

## Future Scope

### Short-term Enhancements
1. **Emergency Access Protocol**: Implement emergency override for critical situations with proper audit trails
2. **Record Categories**: Categorize records by type (lab results, prescriptions, imaging, consultations)
3. **File Attachments**: Support IPFS integration for storing medical images and documents
4. **Prescription Management**: Dedicated module for prescription tracking and pharmacy integration

### Medium-term Developments
1. **Multi-signature Records**: Require multiple doctor signatures for sensitive procedures
2. **Insurance Integration**: Allow insurance providers controlled access for claims processing
3. **Appointment Scheduling**: Integrate appointment booking with record access
4. **Analytics Dashboard**: Provide anonymized health analytics for research purposes
5. **Mobile Application**: Develop patient and doctor mobile apps for easy access

### Long-term Vision
1. **AI Integration**: Implement AI-powered diagnosis assistance and health predictions
2. **Cross-chain Interoperability**: Enable record sharing across different blockchain networks
3. **Global Health Network**: Build a worldwide network of healthcare providers
4. **Genomic Data Storage**: Secure storage and management of genetic information
5. **Telemedicine Integration**: Full integration with telehealth platforms
6. **IoT Device Integration**: Connect wearable devices for continuous health monitoring
7. **Clinical Trial Management**: Facilitate patient recruitment and data collection for research
8. **Pharmaceutical Tracking**: Track medication supply chain from manufacturer to patient

### Research Areas
- Zero-knowledge proofs for enhanced privacy
- Quantum-resistant cryptography for future-proofing
- Machine learning on encrypted medical data
- Decentralized identity (DID) integration
- Layer 2 scaling solutions for lower transaction costs

---

## Technical Stack

- **Smart Contract Language**: Solidity ^0.8.0
- **Blockchain**: Ethereum (compatible with EVM chains)
- **Development Framework**: Hardhat/Truffle
- **Testing**: Mocha/Chai

## Getting Started

### Prerequisites
- Node.js v14+
- npm or yarn
- MetaMask or similar Web3 wallet

### Installation
```bash
npm install
```

### Compilation
```bash
npx hardhat compile
```

### Testing
```bash
npx hardhat test
```

### Deployment
```bash
npx hardhat run scripts/deploy.js --network <network-name>
```

## Smart Contract Functions

### Patient Functions
- `registerPatient(string _name)` - Register as a new patient
- `authorizeDoctor(address _doctor)` - Grant access to a doctor<img width="1920" height="1080" alt="Screenshot (27)" src="https://github.com/user-attachments/assets/dab469b3-127c-487e-870c-eba8b3f2b05c" />
<img width="1920" height="1080" alt="Screenshot (27)" src="https://github.com/user-attachments/assets/ece0f19c-41b4-46f7-8c25-6712743754e6" />

- `revokeDoctor(address _doctor)` - Revoke doctor's access
- `getPatientRecords(address _patient)` - View your medical records

### Doctor Functions
- `createMedicalRecord(address _patient, string _diagnosis, string _treatment)` - Create a new medical record

### Admin Functions
- `verifyDoctor(address _doctorAddress, string _name, string _specialization)` - Verify a healthcare provider

## License

MIT License

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## Contact

For questions and support, please open an issue in the repository.

---

**Note**: This is a proof-of-concept implementation. For production use, additional security audits, regulatory compliance checks, and extensive testing are required.
