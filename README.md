<div align="center">
    <a href="#" target="_blank">
        <img src="https://raw.githubusercontent.com/appcypher/gigamono-assets/main/avatar-gigamono-boxed.png" alt="Gigamono Logo" width="140" height="140"></img>
    </a>
</div>

<h1 align="center">Compiler Workflow</h1>

##

`compiler_workflow`
 takes a **workflow graph** (`.wg`) as input and runs a semantic analysis phase and generates JavaScript or WebAssembly code and source maps.

The workflow graph is uses typed language and its semantics is based on Raccoon.

When generating wasm code, any JavaScript module dependency is accessed via the host interface `gigamono/js_call` which is expected to be implemented by a gigamono implementation.
