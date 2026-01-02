# GoGroq

A **tiny (< 200 LOC) Go wrapper** for the Groq LLM API

- One‑function call to send prompts and get responses.  
- No dependencies beyond the std‑lib and a single HTTP client.  
- Designed to stay simple, readable, and easy to embed in any Go project.

## Build

```
go install github.com/4sp1/GoGroq@latest
```

You can also explore [GOOS
and GOARCH](https://pkg.go.dev/internal/platform#pkg-variables) to choose the
platform you’d like to target—whether it’s Windows, Linux, macOS, or any other
supported system.

## Use

If you’re a \*‑nix user, you’ll see how to customize your usage:
```
GoGroq -h
```

For anyone who feels a little hesitant about diving into the terminal

1. **Configuration**
   - Generates a `key.txt` file where you copy your Groq API key.
   - Generates a `user.txt` file to populate with your prompt.
   - Run the configuration command:

     ```bash
     GoGroq.exe -config
     ```

     or

     ```bash
     GoGroq -config
     ```

2. Make sure your key is saved in `key.txt`

3. Edit `user.txt`, then double‑click `GoGroq.exe`. After the terminal window
   closes, the file `response.txt` will be created.
