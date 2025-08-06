██████╗██████╗  █████╗  ██████╗██╗  ██╗███████╗███╗   ███╗██╗████████╗██╗  ██╗
██╔════╝██╔══██╗██╔══██╗██╔════╝██║ ██╔╝██╔════╝████╗ ████║██║╚══██╔══╝██║  ██║
██║     ██████╔╝███████║██║     █████╔╝ ███████╗██╔████╔██║██║   ██║   ███████║
██║     ██╔══██╗██╔══██║██║     ██╔═██╗ ╚════██║██║╚██╔╝██║██║   ██║   ██╔══██║
╚██████╗██║  ██║██║  ██║╚██████╗██║  ██╗███████║██║ ╚═╝ ██║██║   ██║   ██║  ██║
 ╚═════╝╚═╝  ╚═╝╚═╝  ╚═╝ ╚═════╝╚═╝  ╚═╝╚══════╝╚═╝     ╚═╝╚═╝   ╚═╝   ╚═╝  ╚═╝

# CrackSmith - Advanced Password Wordlist Generator

[![Python Version](https.img.shields.io/badge/python-3.8%2B-blue.svg)](https://python.org)
[![License](https.img.shields.io/badge/license-MIT-green.svg)](LICENSE)
[![Build Status](https.img.shields.io/badge/build-passing-brightgreen.svg)]()
[![Security](https.img.shields.io/badge/security-pentesting-red.svg)]()

> **A next-generation CLI wordlist generator for cybersecurity professionals, penetration testers, and security researchers.**

CrackSmith is an advanced Python-based command-line tool inspired by CUPP (Common User Passwords Profiler) but enhanced with modern features, intelligent algorithms, and professional-grade capabilities. Designed specifically for ethical hacking, penetration testing, and security research scenarios.

---

## 🚀 Features

### 🎯 **Advanced Target Profiling**
- **Interactive Profiling Mode**: Comprehensive questionnaire system for target information
- **Smart Data Collection**: Names, birthdates, anniversaries, pets, favorite words, locations
- **Relationship Mapping**: Family members, friends, colleagues, and significant others
- **Social Engineering Intelligence**: Company names, job titles, hobbies, and interests

### 🔄 **Intelligent Transformations**
- **Leetspeak Engine**: Advanced 1337 speak transformations with multiple variants
- **Case Variations**: Upper, lower, title, alternating, and random case patterns
- **Character Substitution**: Smart replacement of common characters (@ for a, 3 for e, etc.)
- **Reverse Engineering**: Backward strings and mirror transformations

### ⚙️ **Rule-Based Generation**
- **Custom Rule Engine**: Define your own transformation rules
- **Pattern Recognition**: Automatic detection of common password patterns
- **Permutation Algorithms**: Advanced combination and permutation logic
- **Smart Appending**: Years, numbers, special characters with intelligent placement

### 🎛️ **Multi-Level Generation Modes**
- **Basic Mode**: Simple combinations and common patterns
- **Intermediate Mode**: Enhanced transformations and moderate complexity
- **Advanced Mode**: Maximum permutations with all transformation rules
- **Custom Mode**: User-defined rules and transformation sets

### 🖥️ **Professional CLI Interface**
- **Colored Output**: Beautiful, readable terminal interface with syntax highlighting
- **ASCII Art Banners**: Professional branding and visual appeal
- **Progress Bars**: Real-time generation progress with ETA calculations
- **Live Statistics**: Word count, generation speed, and completion metrics

### 📊 **Advanced Analytics**
- **Generation Statistics**: Detailed metrics on wordlist composition
- **Pattern Analysis**: Breakdown of transformation types and frequencies
- **Performance Metrics**: Generation speed, memory usage, and efficiency stats
- **Export Reports**: Detailed generation reports in multiple formats

### 🔧 **Enhanced Functionality**
- **Wordlist Import**: Extend existing wordlists with new transformations
- **Dry Run Mode**: Preview generation without creating files
- **Multiple Output Formats**: .txt, .zip, .gz compression support
- **Multithreading**: Optional parallel processing for large wordlists
- **Memory Optimization**: Efficient handling of large datasets

### 🔒 **Security & Compliance**
- **Ethical Use Framework**: Built-in guidelines and warnings
- **Audit Logging**: Comprehensive logging of all generation activities
- **Rate Limiting**: Prevent resource abuse and system overload
- **Legal Compliance**: Adherence to responsible disclosure principles

---

## 📦 Installation

### Prerequisites
- **Python 3.8+** (recommended: Python 3.9 or higher)
- **pip** package manager
- **Git** (for cloning repository)

### Method 1: Git Clone (Recommended)
```bash
# Clone the repository
git clone https://github.com/yourusername/cracksmith.git
cd cracksmith

# Create virtual environment (recommended)
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Make executable (Linux/macOS)
chmod +x cracksmith.py
```

### Method 2: Pip Install (Coming Soon)
```bash
# Install from PyPI
pip install cracksmith

# Or install from GitHub directly
pip install git+https://github.com/yourusername/cracksmith.git
```

### Method 3: Development Setup
```bash
# Clone and install in development mode
git clone https://github.com/yourusername/cracksmith.git
cd cracksmith
pip install -e .
```

### Dependencies
```
colorama>=0.4.4
tqdm>=4.62.0
click>=8.0.0
pyfiglet>=0.8.0
rich>=10.0.0
```

---

## 🎮 Usage

### Basic Usage
```bash
# Interactive mode (recommended for beginners)
python cracksmith.py --interactive

# Quick generation with target name
python cracksmith.py --target "john smith" --output john_wordlist.txt

# Advanced mode with all transformations
python cracksmith.py --target "jane doe" --mode advanced --output jane_advanced.txt
```

### Command Line Interface
```bash
python cracksmith.py [OPTIONS]

Options:
  -t, --target TEXT           Target name or identifier
  -o, --output TEXT          Output filename (default: wordlist.txt)
  -m, --mode [basic|intermediate|advanced|custom]
                             Generation complexity mode
  -i, --interactive          Launch interactive profiling mode
  -d, --dry-run             Preview generation without creating files
  -c, --compress [zip|gz]    Compress output file
  -j, --threads INTEGER      Number of threads for parallel processing
  -v, --verbose             Enable verbose logging
  -q, --quiet               Suppress all output except errors
  --import-wordlist TEXT     Import existing wordlist to extend
  --max-length INTEGER       Maximum password length (default: 16)
  --min-length INTEGER       Minimum password length (default: 4)
  --no-symbols              Exclude special characters
  --no-numbers              Exclude numeric characters
  --leetspeak-only          Generate only leetspeak variants
  --stats                   Show detailed generation statistics
  --config TEXT             Load configuration from file
  --help                    Show this message and exit
```

### Interactive Mode
```bash
python cracksmith.py --interactive
```
The interactive mode will guide you through a comprehensive profiling questionnaire:
- Personal information (names, nicknames, surnames)
- Important dates (birthdays, anniversaries)
- Personal interests (hobbies, favorite things)
- Professional information (company, job title)
- Family and relationships
- Locations and addresses
- Custom words and phrases

---

## 💡 Examples

### Example 1: Basic Personal Wordlist
```bash
# Generate basic wordlist for target "John Smith" born in 1985
python cracksmith.py --target "john smith" --mode basic --output john_basic.txt

# Sample output preview:
# john
# smith
# johnsmith
# john1985
# smith1985
# john85
# johnsmith85
```

### Example 2: Advanced Corporate Target
```bash
# Advanced wordlist for corporate penetration testing
python cracksmith.py \
  --target "sarah johnson" \
  --mode advanced \
  --output sarah_corporate.txt \
  --compress zip \
  --threads 4 \
  --stats

# Includes transformations like:
# sarahjohnson
# SarahJohnson
# sarah.johnson
# s4r4hj0hn50n
# sarahj123
# johnson2023
```

### Example 3: Interactive Comprehensive Profiling
```bash
python cracksmith.py --interactive --mode advanced --output comprehensive.txt

# Interactive session will collect:
# - Full name: Sarah Elizabeth Johnson
# - Nickname: Saz, SJ
# - Birthday: March 15, 1990
# - Pet: Max (dog)
# - Company: TechCorp
# - Hobbies: Photography, hiking
# - Favorite color: Blue
# - Anniversary: June 20, 2015
```

### Example 4: Extending Existing Wordlist
```bash
# Import and enhance existing wordlist
python cracksmith.py \
  --import-wordlist existing_passwords.txt \
  --target "mike wilson" \
  --mode intermediate \
  --output enhanced_wordlist.txt \
  --compress gz
```

### Example 5: Dry Run and Statistics
```bash
# Preview generation without creating files
python cracksmith.py \
  --target "alex brown" \
  --mode advanced \
  --dry-run \
  --stats \
  --verbose

# Output shows:
# - Estimated wordlist size
# - Transformation breakdown
# - Generation time estimate
# - Memory usage prediction
```

### Example 6: Custom Configuration
```bash
# Use custom configuration file
python cracksmith.py \
  --config profiles/corporate.json \
  --target "emma davis" \
  --output emma_custom.txt

# corporate.json contains:
# - Custom transformation rules
# - Specific character sets
# - Company-specific patterns
# - Industry terminology
```

---

## 🔧 Advanced Configuration

### Configuration File Format
Create a JSON configuration file for custom generation rules:

```json
{
  "generation_mode": "advanced",
  "transformations": {
    "leetspeak": true,
    "case_variations": true,
    "reverse": true,
    "append_years": [2020, 2021, 2022, 2023, 2024],
    "append_numbers": [1, 12, 123, 1234],
    "special_chars": ["!", "@", "#", "$", "%"]
  },
  "filters": {
    "min_length": 6,
    "max_length": 20,
    "exclude_common": true,
    "require_complexity": false
  },
  "output": {
    "format": "txt",
    "compression": "none",
    "sort_alphabetically": true,
    "remove_duplicates": true
  }
}
```

### Custom Rules Engine
Define custom transformation rules:

```python
# custom_rules.py
def custom_transformation(word):
    """Custom transformation function"""
    transformations = []
    
    # Add year variations
    for year in range(1980, 2025):
        transformations.append(f"{word}{year}")
        transformations.append(f"{word}{str(year)[-2:]}")
    
    # Add company-specific patterns
    companies = ["corp", "inc", "ltd", "llc"]
    for company in companies:
        transformations.append(f"{word}{company}")
        transformations.append(f"{word}.{company}")
    
    return transformations
```

---

## 📊 Output Formats and Statistics

### Standard Output
```
Generated wordlist: target_wordlist.txt
Total passwords: 15,847
Generation time: 2.34 seconds
File size: 245 KB
Compression ratio: 67% (if compressed)

Transformation breakdown:
├── Base words: 23
├── Case variations: 1,456
├── Leetspeak: 2,891
├── Number combinations: 4,567
├── Special characters: 3,234
├── Reverse patterns: 1,876
└── Custom rules: 1,800

Performance metrics:
├── Generation speed: 6,773 passwords/second
├── Memory usage: 45.2 MB peak
├── CPU utilization: 78% average
└── Thread efficiency: 94%
```

### Detailed Statistics Report
```bash
python cracksmith.py --target "example" --stats --output-stats report.json
```

Generates comprehensive JSON report with:
- Generation metadata
- Transformation statistics
- Performance metrics
- Quality analysis
- Duplicate detection results

---

## 🛠️ Development and Contributing

### Development Setup
```bash
# Clone repository
git clone https://github.com/yourusername/cracksmith.git
cd cracksmith

# Create development environment
python -m venv dev-env
source dev-env/bin/activate

# Install development dependencies
pip install -r requirements-dev.txt

# Install pre-commit hooks
pre-commit install

# Run tests
python -m pytest tests/
```

### Code Style and Standards
- **PEP 8** compliance for Python code
- **Type hints** for all function signatures
- **Docstrings** for all public methods and classes
- **Unit tests** with minimum 80% coverage
- **Security-first** development approach

### Contributing Guidelines
1. **Fork** the repository
2. **Create** a feature branch (`git checkout -b feature/amazing-feature`)
3. **Commit** your changes (`git commit -m 'Add amazing feature'`)
4. **Push** to the branch (`git push origin feature/amazing-feature`)
5. **Open** a Pull Request

### Reporting Issues
- Use the **GitHub Issues** tracker
- Provide **detailed reproduction steps**
- Include **system information** and **error logs**
- Follow the **issue template** format

### Feature Requests
- Check **existing issues** first
- Provide **clear use cases** and **benefits**
- Consider **implementation complexity**
- Discuss **security implications**

---

## 🔒 Security and Legal Considerations

### Ethical Use Policy
CrackSmith is designed for **legitimate security testing** and **authorized penetration testing** only. Users must:

- ✅ **Obtain proper authorization** before testing any systems
- ✅ **Comply with local laws** and regulations
- ✅ **Follow responsible disclosure** practices
- ✅ **Respect privacy** and confidentiality
- ❌ **Never use for malicious purposes**
- ❌ **Never test systems without permission**

### Legal Disclaimer
This tool is provided for **educational and authorized security testing purposes only**. The developers are not responsible for any misuse or illegal activities performed with this software. Users are solely responsible for ensuring their use complies with applicable laws and regulations.

### Security Features
- **No data collection**: All processing is performed locally
- **No network communication**: Tool operates entirely offline
- **Secure deletion**: Temporary files are securely removed
- **Audit logging**: All activities are logged for compliance

---

## 📄 License

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

```
MIT License

Copyright (c) 2024 CrackSmith Contributors

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

---

## 🤝 Acknowledgments

- **CUPP Project**: Original inspiration and foundational concepts
- **Security Community**: Feedback, testing, and feature suggestions
- **Open Source Contributors**: Code contributions and improvements
- **Penetration Testing Community**: Real-world use cases and requirements

---

## 📞 Support and Contact

- **GitHub Issues**: [Report bugs and request features](https://github.com/yourusername/cracksmith/issues)
- **Documentation**: [Comprehensive guides and tutorials](https://github.com/yourusername/cracksmith/wiki)
- **Security Issues**: [Responsible disclosure](mailto:security@cracksmith.com)
- **General Questions**: [Community discussions](https://github.com/yourusername/cracksmith/discussions)

---

## 🚀 Roadmap

### Version 2.0 (Planned)
- [ ] **Machine Learning Integration**: AI-powered password pattern prediction
- [ ] **Web Interface**: Browser-based GUI for easier usage
- [ ] **API Endpoints**: RESTful API for integration with other tools
- [ ] **Database Support**: Direct integration with password databases
- [ ] **Cloud Processing**: Optional cloud-based generation for large datasets

### Version 2.1 (Future)
- [ ] **Mobile App**: iOS and Android companion applications
- [ ] **Team Collaboration**: Multi-user project management
- [ ] **Advanced Analytics**: Detailed password strength analysis
- [ ] **Integration Plugins**: Direct integration with popular pentesting frameworks

---

**⚡ Happy Hacking! Stay Ethical, Stay Legal! ⚡**

---

<div align="center">
  <sub>Built with ❤️ by the cybersecurity community for the cybersecurity community</sub>
</div>
