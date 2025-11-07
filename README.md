# ================================
# Project: codeForge reliable Powerhouse
# Description:
# A powerhouse repository where new ideas are forged into working code.
# Built for experimentation, innovation, and reliable development.
# ================================

# ---------- main.py ----------
"""
Main  point for the CodeForge Powerhouse.
"""

from core import forge, reliability


def run():
    print("🔥 Welcome to the CodeForge Powerhouse")
    print("⚙️ Forging new ideas into reliable code.\n")

    # Try out features
    idea = "innovation"
    print(f"🛠️ Forged Idea (reverse): {forge.reverse_text(idea)}")
    print("🧩 Forged Pattern:\n", forge.pattern(5))
    print("🛡️ Reliable Utility (safe divide):", reliability.safe_divide(42, 0))


if __name__ == "__main__":
    run()


# ---------- core/forge.py ----------
"""
Module for forging ideas into working code: experiments and prototypes.
"""

def reverse_text(text: str) -> str:
    """Reverse a string."""
    return text[::-1]

def pattern(n: int) -> str:
    """Create a simple text pattern."""
    return "\n".join("*" * i for i in range(1, n + 1))


# ---------- core/reliability.py ----------
"""
Module for reliable utilities, error handling, and stable helpers.
"""

def safe_divide(a: float, b: float):
    """Divide safely, return None if division by zero."""
    try:
        return a / b
    except ZeroDivisionError:
        return None 

def ensure_positive(n: float) -> float:
    """Ensure a number is positive."""
    return abs(n)


# ---------- tests/test_reliability.py ----------
"""
Basic tests for reliability.py
Run with: pytest
"""

from core import reliability

def t
