# Validation run 2026-08-24

### Pattern Check

**Status:** PASS

**Notes:** The canonical cookbook checker validated all 9 examples with no
violations.

### async_toolkit_context.py

**Status:** PASS

**Description:** Deterministic execution verifying that async-only toolkit
functions are included in the team members system message.

**Result:** PASS. Both `async_search` and `async_summarize` were present. No API
key, model call, database, or external service was required.

---

# Validation run 2026-02-15T00:43:27

### Pattern Check

**Status:** PASS

**Notes:** No pattern violations detected.

### OpenAIChat references

**Found in:**
- TEST_LOG.md

---

### async_tools.py

**Status:** FAIL

**Description:** Example execution attempt

**Result:** FAIL. Traceback (most recent call last):
  File "/Users/ab/conductor/workspaces/agno/tallinn/libs/agno/agno/tools/agentql.py", line 8, in <module>
    import agentql
ModuleNotFoundError: No module named 'agentql'

During handling of the above exception, another exception occurred:

Traceback (most recent call last):
  File "/Users/ab/conductor/workspaces/agno/tallinn/cookbook/03_teams/03_tools/async_tools.py", line 14, in <module>
    from agno.tools.agentql import AgentQLTools
  File "/Users/ab/conductor/workspaces/agno/tallinn/libs/agno/agno/tools/agentql.py", line 11, in <module>
    raise ImportError("`agentql` not installed. Please install using `pip install agentql`")
ImportError: `agentql` not installed. Please install using `pip install agentql`

---

### custom_tools.py

**Status:** PASS

**Description:** Example executed (demo run)

**Result:** PASS

---

### member_information.py

**Status:** PASS

**Description:** Example executed (demo run)

**Result:** PASS

---

### member_tool_hooks.py

**Status:** PASS

**Description:** Example executed (demo run)

**Result:** PASS

---

### tool_call_limit.py

**Status:** PASS

**Description:** Example executed (demo run)

**Result:** PASS

---

### tool_choice.py

**Status:** PASS

**Description:** Example executed (demo run)

**Result:** PASS

---

### tool_hooks.py

**Status:** FAIL

**Description:** Example execution attempt

**Result:** FAIL. Timeout after 120s

---
