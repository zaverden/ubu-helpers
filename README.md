# ubu-helpers

```bash
cp ~/.bashrc ~/.bashrc_bkp

echo "
HELPERS_DIR=${PWD}
if [ -f \${HELPERS_DIR}/bash/aliases ]; then
    . \${HELPERS_DIR}/bash/aliases
fi

if [ -f \${HELPERS_DIR}/bash/prompt ]; then
    . \${HELPERS_DIR}/bash/prompt
fi

PATH=\"\$HELPERS_DIR:\$PATH\"

" >> ~/.bashrc

cp bash/completion ~/.bash_completion
```
