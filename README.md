## Installation and Setup Instructions

Follow these steps to set up the project on your system.

### Step 1: Update Package Lists

```sh
sudo apt update
```

- **Description**: Updates the list of available packages and their versions.

### Step 2: Install Required Packages

```sh
sudo apt install git make autoconf g++ flex bison libcurl4-openssl-dev autoconf help2man iverilog
```

- **Description**: Installs the necessary packages for building and running Verilator and other dependencies.

### Step 3: Clone the Verilator Repository

```sh
git clone https://github.com/verilator/verilator.git
```

- **Description**: Clones the Verilator repository from GitHub.

### Step 4: Navigate to the Verilator Directory

```sh
cd verilator
```

- **Description**: Changes the current directory to the Verilator directory.

### Step 5: Checkout the Stable Branch

```sh
git checkout stable
```

- **Description**: Switches to the stable branch of the Verilator repository.

### Step 6: Generate Configuration Scripts

```sh
autoconf
```

- **Description**: Generates the `configure` script needed to build Verilator.

### Step 7: Configure the Build

```sh
./configure
```

- **Description**: Configures the build environment for Verilator.

### Step 8: Build Verilator

```sh
make
```

- **Description**: Compiles Verilator using 4 parallel jobs to speed up the process.

### Step 9: Install Verilator

```sh
sudo make install
```

- **Description**: Installs Verilator on your system.

### Step 10: Clone the LLM Hardware Test Generation Project

```sh
git clone https://github.com/magicYang1573/llm-hardware-test-generation.git
```

- **Description**: Clones the LLM Hardware Test Generation project repository from GitHub.

### Step 11: Install Python and Virtual Environment

```sh
sudo apt install python3 python3-venv
```

- **Description**: Installs Python 3 and the virtual environment package.

### Step 12: Navigate to the Project Directory

```sh
cd ~/llm-hardware-test-generation
```

- **Description**: Changes the current directory to the project directory.

### Step 13: Create a Virtual Environment

```sh
python3 -m venv venv
```

- **Description**: Creates a virtual environment named `venv`.

### Step 14: Activate the Virtual Environment

```sh
source venv/bin/activate
```

- **Description**: Activates the virtual environment.

### Step 15: Upgrade pip

```sh
pip3 install --upgrade pip
```

- **Description**: Upgrades pip to the latest version.

### Step 16: Install PyVerilog

```sh
pip3 install -r requirements.txt
```

- **Description**: Installs the PyVerilog package.

update run.sh with your openai key
update export VERILATOR_ROOT="/usr/bin/verilator #Path of your verilator

### Step 17: Run the Project

```sh
./run.sh
```

- **Description**: Executes the `run.sh` script to start the project.