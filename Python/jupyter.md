```bash
# Loads the autoreload extension, which automatically reloads modules before executing code.
%load_ext autoreload
# Sets autoreload to reload all modules (except those excluded) every time before executing a new cell. This is useful for development, as changes to imported Python files are picked up without restarting the kernel.
%autoreload 2
```