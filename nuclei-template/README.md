
## Nuclei Templates

### Reflected Host Header Injection - Ultimate Detection

**Template ID**: `reflected-host-header-injection-ultimate-spectorsec`

**Features**:
- Detects reflected Host Header Injection across multiple vectors
- Tests 12 different header variations (Host, X-Forwarded-Host, etc.)
- Checks for reflections in:
  - HTML content
  - Location headers
  - JSON/JavaScript
  - Meta tags
  - CSP/CORS headers
  - Error messages
- Includes common bypass techniques (/%2e/, :443, etc.)

**Usage**:
```bash
nuclei -t hhi.yaml -u https://target.com
