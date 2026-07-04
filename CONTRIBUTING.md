# Contributing to llama.cpp POWER8 Optimization

Thank you for your interest in contributing to this POWER8 optimization project!

## Development Setup

### Requirements
- CMake 3.10+
- GCC with POWER8 VSX support
- Linux (recommended: Ubuntu 20.04+ or RHEL 8+)

### Build Instructions

```bash
# Clone and setup
git clone https://github.com/Scottcjn/llama-cpp-power8.git
cd llama-cpp-power8

# Build with CMake
mkdir build && cd build
cmake .. -DCMAKE_BUILD_TYPE=Release
make -j$(nproc)
```

### Testing

Run the benchmark to verify your changes:

```bash
./bin/benchmark --help
```

## Pull Request Workflow

1. Fork the repository
2. Create a feature branch: `git checkout -b feat/your-feature`
3. Make your changes and test
4. Submit a Pull Request
5. Wait for review and merging

## Code Style

- Follow existing code patterns
- Add comments for POWER8-specific optimizations
- Test on real POWER8 hardware when possible

## Resources

- [llama.cpp main repo](https://github.com/ggerganov/llama.cpp)
- [POWER8 VSX documentation](https://www.ibm.com/docs/en/linux-on-z/14.02?topic=concepts-vsx)
