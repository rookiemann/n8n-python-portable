# n8n 1.123.5 + Python 3.14 – Fully Portable Windows

No Docker • No pip • No conda • No admin rights • Works offline

Extract → double-click `start-n8n.bat` → open http://localhost:5678  
Native **Python Code** node works instantly.

### Download
[Latest ZIP](https://github.com/rookiemann/n8n-python-portable/releases/latest/download/n8n-python-portable.zip) (~383 MB)

### Folder Structure

```
n8n-python-portable/                          # Extract this folder anywhere
│
├── start-n8n.bat                             # Double-click this to launch n8n
├── package.json                              # n8n config
├── package-lock.json                         # Locked deps
│
├── node/                                     # Bundled Node.js (no install needed)
│   ├── node.exe                              # Runs n8n
│   ├── npm.cmd                               # Optional package manager
│   └── ...                                   # Other Node files
│
├── python/                                   # Fully embedded Python 3.14
│   ├── python.exe                            # The Python interpreter
│   ├── python314.dll                         # Core DLL
│   ├── python314._pth                        # Path config for portability
│   ├── DLLs/                                 # Dynamic libraries
│   │   ├── sqlite3.dll
│   │   ├── _ssl.pyd
│   │   └── ...
│   ├── Lib/                                  # Standard library (full Python stdlib)
│   │   ├── site-packages/                    # For any extra modules
│   │   ├── asyncio/
│   │   ├── collections/
│   │   └── ...
│   └── Scripts/                              # Tools like pip (optional)
│       └── pip.exe
│
├── node_modules/                             # 100% complete n8n dependencies
│   ├── n8n/                                  # n8n core
│   │   └── bin/n8n                           # CLI entrypoint
│   ├── @n8n/                                 # n8n extensions
│   ├── @langchain/                           # AI/LLM support
│   ├── axios/                                # HTTP client
│   ├── express/                              # Web server
│   ├── ...                                   # ~4000+ packages
│
└── .n8n/                                     # Created on first run (your data)
    ├── config                                # Settings
    ├── database.sqlite                       # Workflow storage
    └── workflows/                            # Saved automations
```
    
