# Simple Interest Calculator

A project to create a command-line tool for calculating simple interest using a Bash script. This repository was created as a requirement for the IBM Data Science Professional Certificate.

## About The Project

This project provides the functionality to calculate simple interest based on user-provided inputs.

### Project Description:

> A calculator that calculates simple interest given principal, annual rate of interest and time period in years.

#### Input:
* `p`: principal amount
* `t`: time period in years
* `r`: annual rate of interest

#### Output:
* The script will calculate and return the simple interest based on the formula: `simple interest = p * t * r`

---

## The Program to Implement

The main task is to create a shell script named `simple-interest.sh` in the root of the repository with the exact following content.

#### Script Code (`simple-interest.sh`):
```bash
#!/bin/bash
# This script calculates simple interest given principal,
# annual rate of interest and time period in years.
# Do not use this in production. Sample purpose only.

# Author: Upkar Lidder (IBM)
# Additional Authors:
# monica606003

# Input:
# p, principal amount
# t, time period in years
# r, annual rate of interest

# Output:
# simple interest = p*t*r

echo "Enter the principal:"
read p
echo "Enter rate of interest per year:"
read r
echo "Enter time period in years:"
read t

s=`expr $p \* $t \* $r / 100`

echo "The simple interest is: "
echo $s
```

---

## Getting Started

### Prerequisites

You will need a terminal environment that can run Bash scripts (Linux, macOS, or Git Bash/WSL on Windows).

### Installation

1.  Clone this repository to your local machine:
    ```sh
    git clone https://github.com/bledxs/github-final-project.git
    ```
2.  Navigate to the project directory:
    ```sh
    cd github-final-project
    ```

---

## Usage Guide

Once the `simple-interest.sh` file is created:

1.  **Make the script executable** (one-time command):
    ```sh
    chmod +x simple-interest.sh
    ```
2.  **Run the script:**
    ```sh
    ./simple-interest.sh
    ```

#### Example Interaction:
```
$ ./simple-interest.sh
Enter the principal:
1000
Enter rate of interest per year:
5
Enter time period in years:
2
The simple interest is: 
100
```

---

## Contributing

Contributions are welcome. Please read the `CONTRIBUTING.md` file for details on our code of conduct and the process for submitting pull requests.

## License

This project is distributed under the Apache 2.0 License. See `LICENSE` and `NOTICE` for more information.
