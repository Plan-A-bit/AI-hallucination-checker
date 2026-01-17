# Hallucination Tester

A GUI-based tool for detecting hallucinations in LLM responses using your existing `llmcheck` verification script.
It use Keywords to detect.

## Prerequisites

- Python 3.6+
- PyQt5
- Your existing `llmcheck` script (must be in PATH)

### Installing PyQt5

On Fedora:
```bash
sudo dnf install python3-qt5 or pip3 install PyQt5

#### Installation

    Clone the repository:

git clone https://github.com/Plan-A-bit/hallucination-tester.git
cd hallucination-tester
chmod +x hallucination_tester.py

test using
echo "test response" | llmcheck

Launch it independantly from local host LLM or any other AI
python3 hallucination_tester.py

Manual
Paste LLM responses in the input text area
Click "Test for Hallucinations" to run verification
Results show:

    ✓ TRUSTED RESPONSE (no hallucinations)
    ! FLAGGED RESPONSE (hallucinations detected)

Use "Clear" to reset the interface
Done!

