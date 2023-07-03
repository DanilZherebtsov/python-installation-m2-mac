# python-installation-m2-mac

# Code snippets to copy/paste:
# -------------------------------------------------------------------------------------

# Pyenv dependencies:
brew install openssl readline sqlite3 xz zlib tcl-tk libffi

# .zshrc config code:
export PYENV_ROOT="$HOME/.pyenv"
command -v pyenv >/dev/null || export PATH="$PYENV_ROOT/bin:$PATH"
eval "$(pyenv init -)"
eval "$(pyenv virtualenv-init -)"
export CONFIGURE_OPTS="--with-openssl=$(brew --prefix openssl)"
export PATH="$PYENV_ROOT/shims:$PATH"
export PATH="$PYENV_ROOT/bin:$PATH"
