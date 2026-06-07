# Setup Instructions - Fuzzy Maker

## Prerequisites

- **Node.js**: 16.0.0+ ([Download](https://nodejs.org/))
- **npm**: 7.0.0+ (included with Node.js) or **yarn**: 1.22.0+
- **Git**: 2.0+

### System Requirements

| OS | Version | Support |
|---|---|---|
| Linux | Any modern distro | ✅ Full |
| macOS | 10.15+ | ✅ Full |
| Windows | 10/11 | ✅ Full |

## Installation

### 1. Clone the Repository

```bash
git clone https://github.com/m74278803-cmyk/fuzzy-maker.git
cd fuzzy-maker
```

### 2. Install Dependencies

Using npm:
```bash
npm install
```

Or using yarn:
```bash
yarn install
```

### 3. Verify Installation

```bash
npm test
```

## Development Setup

### Running Locally

```bash
npm run dev
```

This starts the development server on `http://localhost:3000`

### Building for Production

```bash
npm run build
```

### Running Tests

```bash
# All tests
npm test

# Watch mode
npm test -- --watch

# Coverage
npm test -- --coverage
```

### Code Quality

```bash
# Lint
npm run lint

# Format
npm run format

# Type checking
npm run type-check
```

## Environment Setup

Create `.env.local` file:

```env
NODE_ENV=development
DEBUG=fuzzy-maker:*
API_URL=http://localhost:3000
```

## Troubleshooting

### Issue: `npm ERR! code ENOENT`
**Solution**: Ensure you're in project root
```bash
cd fuzzy-maker
npm install
```

### Issue: Port 3000 already in use
**Solution**: Use different port
```bash
PORT=3001 npm run dev
```

### Issue: Module not found errors
**Solution**: Clear cache and reinstall
```bash
rm -rf node_modules package-lock.json
npm install
```

## Common Commands

```bash
# Install
npm install

# Start dev
npm run dev

# Build
npm run build

# Test
npm test

# Lint
npm run lint

# Format code
npm run format

# Clean
npm run clean
```

## Project Structure

```
fuzzy-maker/
├── src/
│   ├── components/
│   ├── utils/
│   └── index.js
├── tests/
├── public/
├── package.json
└── README.md
```

## Contributing

1. Create feature branch: `git checkout -b feature/name`
2. Install pre-commit hooks: `npm run prepare`
3. Make changes and test: `npm test`
4. Commit: `git commit -am 'Add feature'`
5. Push: `git push origin feature/name`
6. Create Pull Request

## Documentation

- [Node.js Guide](https://nodejs.org/docs/)
- [npm Docs](https://docs.npmjs.com/)
- [Project Docs](./docs)

## Support

For issues:
1. Check [GitHub Issues](https://github.com/m74278803-cmyk/fuzzy-maker/issues)
2. Review [Discussions](https://github.com/m74278803-cmyk/fuzzy-maker/discussions)
