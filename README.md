# Juristatix (Demo App)

Juristatix is a **fictitious demo application** built with the [SignumFlow API](https://signumflow.com).  
It demonstrates how legal teams can streamline **contract approvals**, **deadline tracking**, and **compliance automation**.

---

## ⚠️ Disclaimer

This is **not a production app**.  
Juristatix is a **reference implementation** provided for learning and experimentation.

---

## 🚀 Features

- Multi-step approval workflows  
- Deadline and reminder tracking  
- Compliance automation examples  

---

## 🔗 Resources

- [Live Demo](https://juristatix.signumflow.dev)  
- [Source Code on GitHub](https://github.com/signumfl/Juristatix-Demo-Legal-Workflow-App)  
- [SignumFlow Documentation](https://signumflow.com/docs)

---

## 🛠️ Tech Stack

- **Frontend:** Vanilla JavaScript, HTML5, CSS3  
- **Backend:** Node.js, Express.js  
- **API Integration:** SignumFlow REST API  
- **Authentication:** SignumFlow API Keys  
- **File Upload:** AWS S3 with presigned URLs  
- **Real-time Updates:** Webhooks + Server-Sent Events  

---

## 🔧 Installation & Setup

### Prerequisites

- [Node.js](https://nodejs.org/) 18+ and npm  
- [SignumFlow API account](https://developer.signumflow.com/) (Free trial available)  

### 1. Clone the Repository

```bash
git clone https://github.com/signumflow/Juristatix-Demo-Legal-Workflow-App.git
cd Juristatix-Demo-Legal-Workflow-App
```

### 2. Install Dependencies

```bash
npm install
```

### 3. Environment Configuration

Copy the example environment file and configure your settings:

```bash
cp .env.example .env
```

**Edit .env with your SignumFlow API credentials:**

```env
# SignumFlow API Configuration
SIGNUMFLOW_API_KEY=sk_test_your_api_key_here
SIGNUMFLOW_BASE_URL=https://api.signumflow.com/v1
SIGNUMFLOW_WEBHOOK_SECRET=your_webhook_secret_here

# Application Configuration  
APP_NAME=Juristatix Demo Legal Workflow App
APP_PORT=3000
APP_ENV=development

# Demo Configuration
DEMO_MODE=true
DEMO_APPROVER_EMAIL=<your-test-email>
DEMO_WORKFLOW_ID=wf_UUID
```

### 4. Run the Application

**Development mode with hot reload:**

```bash
npm run dev
```

**Production mode:**

```bash
npm run build
npm start
```

The app will be available at http://localhost:3000

---

## 🧪 Testing

```bash
# Run all tests
npm test

# Run specific test suites
npm run test:unit
npm run test:integration
npm run test:e2e

# Run tests with coverage
npm run test:coverage
```

---

## 🔐 Security Features

- **API Key Authentication:** Secure SignumFlow API integration
- **Webhook Signature Verification:** Cryptographic webhook validation
- **CORS Configuration:** Proper cross-origin request handling
- **Input Validation:** Comprehensive request validation
- **Error Handling:** Secure error responses without data leakage

---

## 🚀 Deployment

### Deploy to Vercel

```bash
npm install -g vercel
vercel --prod
```

### Deploy to Heroku

```bash
git push heroku main
```

### Docker Deployment

```bash
docker build -t juristatix-demo-legal-workflow-app .
docker run -p 3000:3000 --env-file .env juristatix-demo-legal-workflow-app
```

---

## 🎨 Customization

This demo is designed to be easily customizable for your specific use case:

- **Workflow Configuration:** Modify `config/workflows.js`
- **UI Components:** Update components in `src/js/components/`
- **Styling:** Customize CSS in `src/css/`
- **Business Logic:** Adapt handlers in `server/routes/`

---

## 📖 Documentation

- [API Documentation](https://signumflow.com/docs) — SignumFlow API integration details

---

## 🤝 Contributing

We welcome contributions! Please see our [Contributing Guidelines](CONTRIBUTING.md) for details.

---

## 📝 License

This project is licensed under the [MIT License](LICENSE).

---

## 🆘 Support

- **Documentation:** [docs.signumflow.com](https://signumflow.com/docs)
- **API Support:** support@signumflow.com
- **Demo Issues:** [GitHub Issues](https://github.com/signumflow/Juristatix-Demo-Legal-Workflow-App/issues)
- **Community:** Join the SignumFlow Discord (link coming soon)

---

