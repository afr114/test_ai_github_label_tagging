## AI Assistance

Select the most relevant level of GenAI assistance used in this PR.  
(Required if this PR involved tools like GitHub Copilot, ChatGPT, etc.)

---

- [ ] **Light** — “I knew what I wanted, AI just filled it in.”

**Definition:**  
Code suggestions or completions based on existing context  
e.g., inline suggestions, autocompleting property names, filling in parameters

**Rule of Thumb:**  
You were already typing the code, and the AI just sped it up or finished it for you.

Examples:
- Typing `user.` in a React component and Copilot suggests `email` based on prop structure
- Suggesting `useEffect(() => {}, [dependency])` after typing `useEff...`
- Autocompleting `render()` method props in a React component
- Suggesting `expect(user.name).to eq("Alice")` in a test file
- Autocompleting `validates :email,` in a Rails model based on typical validations

---

- [ ] **Medium** — “I had something to build, and AI wrote a meaningful chunk for me.”

**Definition:**  
Local code generation or modification e.g., rewriting a function, generating a test case, renaming code, suggesting patterns

**Rule of Thumb:**  
You had the structure or intent in mind, and AI helped you implement or refactor it.

Examples:
- Copilot rewrites a `handleSubmit` function in React to use `async/await` and error handling
- Generates a complete RSpec or Jest test from method signature and context
- Refactors a Ruby class method or suggests converting a React component from `useState` to `useReducer`
- Suggests or inserts JSDoc/YARD comments based on method implementation
- Generates multiple lines of parameter validation in a Rails controller using known params pattern

---

- [ ] **Heavy** — “I wrote a stub or file and AI did all the work, or structured the solution.”

**Definition:**  
New logic, structure, or design decisions e.g., AI-generated architecture, scaffolding new components or jobs, multi-step logic generation

**Rule of Thumb:**  
AI produced the initial structure or solution — even if you revised it afterward.

Examples:
- Starting a new React component file and Copilot scaffolds a full `ModalManager` using reducer/context
- Creating a new Rails job (`send_weekly_digest_job.rb`) and Copilot generates the full `perform` method with mailer logic
- Typing `def reset_password(user)` and Copilot generates token generation, DB updates, and mailer delivery
- Starting a new GraphQL mutation and Copilot scaffolds argument parsing, validation, model updates, and response
- Starting a test file (`authentication_flow_spec.rb`) and Copilot scaffolds test cases for sign-in, sign-out, and password reset
- Creating a new service object (`CheckoutProcessor`) and Copilot generates the class, `initialize`, and `call` method
