# Real-Time Password Evaluator & Generator

A client-side security and entropy analysis tool designed to evaluate real-world password resilience against dictionary attacks, keyboard spatial patterns, and offline cracking rigs.

## Features

**Real-Time Entropy Analysis:** Computes bit entropy ($\approx \log_2(\text{guesses})$) and maps numeric scores from 0 to 100.
**Pattern Recognition:** Leverages Dropbox's `zxcvbn` engine to flag common dictionary words, keyboard layouts (e.g., QWERTY sequences), l33tspeak substitutions, and repeated characters.
**Crack Time Estimations:** Calculates realistic time-to-crack metrics across throttled online login vectors and heavy offline GPU hash-cracking rigs (e.g., bcrypt/Argon2).
**Secure Password Generator:** Generates high-entropy passwords locally utilizing the browser's cryptographically secure pseudo-random number generator (`window.crypto.getRandomValues`).
**Client-Side Privacy:** Zero network calls or backend storage—all calculations execute entirely in the client browser.

## Tech Stack

**Frontend:** HTML5, Tailwind CSS (via CDN)
**Scripting:** Vanilla JavaScript (ES6+)
**Libraries:** 
  [`zxcvbn`](https://github.com/dropbox/zxcvbn) for pattern-matching security heuristics.
  [`Lucide`](https://lucide.dev/) for UI iconography.

## Getting Started Locally

To run this project locally, no complex build steps or package managers are required:

   Clone the repository:
   git clone [https://github.com/kalebshanklin02/password-strength-evaluator.git]
   cd password-strength-evaluator
   #On macOS
   open index.html
   #On Linux
   xdg-open index.html
   
