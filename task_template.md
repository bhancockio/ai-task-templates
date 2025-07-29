# AI Task Template

> **Instructions:** This template helps you create comprehensive task documents for AI-driven development. Fill out each section thoroughly to ensure the AI agent has all necessary context and can execute the task systematically.

---

## 1. Task Overview

### Task Title
<!-- Provide a clear, specific title for this task -->
**Title:** [Brief, descriptive title of what you're building/fixing]

### Goal Statement
<!-- One paragraph describing the high-level objective -->
**Goal:** [Clear statement of what you want to achieve and why it matters]

---

## 2. Strategic Analysis & Solution Options

### When to Use Strategic Analysis
<!-- 
AI Agent: Use your judgement to determine when strategic analysis is needed vs direct implementation.

**✅ CONDUCT STRATEGIC ANALYSIS WHEN:**
- Multiple viable technical approaches exist
- Trade-offs between different solutions are significant
- User requirements could be met through different UX patterns
- Architectural decisions will impact future development
- Implementation approach affects performance, security, or maintainability significantly
- Change touches multiple systems or has broad impact
- User has expressed uncertainty about the best approach

**❌ SKIP STRATEGIC ANALYSIS WHEN:**
- Only one obvious technical solution exists
- It's a straightforward bug fix or minor enhancement 
- The implementation pattern is clearly established in the codebase
- Change is small and isolated with minimal impact
- User has already specified the exact approach they want

**DEFAULT BEHAVIOR:** When in doubt, provide strategic analysis. It's better to over-communicate than to assume.
-->

### Problem Context
<!-- Restate the problem and why it needs strategic consideration -->
[Explain the problem and why multiple solutions should be considered - what makes this decision important?]

### Solution Options Analysis

#### Option 1: [Solution Name]
**Approach:** [Brief description of this solution approach]

**Pros:**
- ✅ [Advantage 1 - specific benefit]
- ✅ [Advantage 2 - quantified when possible]
- ✅ [Advantage 3 - why this is better]

**Cons:**
- ❌ [Disadvantage 1 - specific limitation]
- ❌ [Disadvantage 2 - trade-off or cost]
- ❌ [Disadvantage 3 - risk or complexity]

**Implementation Complexity:** [Low/Medium/High] - [Brief justification]
**Risk Level:** [Low/Medium/High] - [Primary risk factors]

#### Option 2: [Solution Name]
**Approach:** [Brief description of this solution approach]

**Pros:**
- ✅ [Advantage 1]
- ✅ [Advantage 2]
- ✅ [Advantage 3]

**Cons:**
- ❌ [Disadvantage 1]
- ❌ [Disadvantage 2]
- ❌ [Disadvantage 3]

**Implementation Complexity:** [Low/Medium/High] - [Brief justification]
**Risk Level:** [Low/Medium/High] - [Primary risk factors]

#### Option 3: [Solution Name] (if applicable)
**Approach:** [Brief description of this solution approach]

**Pros:**
- ✅ [Advantage 1]
- ✅ [Advantage 2]

**Cons:**
- ❌ [Disadvantage 1]
- ❌ [Disadvantage 2]

**Implementation Complexity:** [Low/Medium/High] - [Brief justification]
**Risk Level:** [Low/Medium/High] - [Primary risk factors]

### Recommendation & Rationale

**🎯 RECOMMENDED SOLUTION:** Option [X] - [Solution Name]

**Why this is the best choice:**
1. **[Primary reason]** - [Specific justification]
2. **[Secondary reason]** - [Supporting evidence]
3. **[Additional reason]** - [Long-term considerations]

**Key Decision Factors:**
- **Performance Impact:** [How this affects app performance]
- **User Experience:** [How this affects users]
- **Maintainability:** [How this affects future development]
- **Scalability:** [How this handles growth]
- **Security:** [Security implications]

**Alternative Consideration:**
[If there's a close second choice, explain why it wasn't selected and under what circumstances it might be preferred]

### Decision Request

**👤 USER DECISION REQUIRED:**
Based on this analysis, do you want to proceed with the recommended solution (Option [X]), or would you prefer a different approach? 

**Questions for you to consider:**
- Does the recommended solution align with your priorities?
- Are there any constraints or preferences I should factor in?
- Do you have a different timeline or complexity preference?

**Next Steps:**
Once you approve the strategic direction, I'll create the detailed implementation plan in the sections below.

---

## 3. Project Analysis & Current State

### Technology & Architecture
<!-- 
AI Agent: Analyze the project to fill this out.
- Check `package.json` for versions and dependencies.
- Check `tsconfig.json` for TypeScript configuration.
- Check `tailwind.config.ts` for styling and theme.
- Check `drizzle/schema/` for database schema.
- Check `middleware.ts` for authentication and routing.
- Check `components/` for existing UI patterns. 
-->
- **Frameworks & Versions:** [e.g., Next.js 15.3, React 19]
- **Language:** [e.g., TypeScript 5.4 with strict mode]
- **Database & ORM:** [e.g., Supabase (Postgres) via Drizzle ORM]
- **UI & Styling:** [e.g., shadcn/ui components with Tailwind CSS for styling]
- **Authentication:** [e.g., Supabase Auth managed by `middleware.ts` for protected routes]
- **Key Architectural Patterns:** [e.g., Next.js App Router, Server Components for data fetching, Server Actions for mutations]
- **Relevant Existing Components:** [e.g., `components/ui/button.tsx` for base styles, `components/auth/LoginForm.tsx` for form patterns]

### Current State
<!-- Describe what exists today based on actual analysis -->
[Describe the current situation, existing code, and what's working/not working - based on actual file analysis, not assumptions]

## 3. Context & Problem Definition

### Problem Statement
<!-- What specific problem are you solving? -->
[Detailed explanation of the problem, including pain points, user impact, and why this needs to be solved now]

### Success Criteria
<!-- How will you know this is complete and successful? -->
- [ ] [Specific, measurable outcome 1]
- [ ] [Specific, measurable outcome 2]
- [ ] [Specific, measurable outcome 3]

---

## 4. Development Mode Context

### Development Mode Context
- **🚨 IMPORTANT: This is a new application in active development**
- **No backwards compatibility concerns** - feel free to make breaking changes
- **Data loss acceptable** - existing data can be wiped/migrated aggressively
- **Users are developers/testers** - not production users requiring careful migration
- **Priority: Speed and simplicity** over data preservation
- **Aggressive refactoring allowed** - delete/recreate components as needed

---

## 5. Technical Requirements

### Functional Requirements
<!-- What should the system do? -->
- [Requirement 1: User can...]
- [Requirement 2: System will...]
- [Requirement 3: When X happens, then Y...]

### Non-Functional Requirements
<!-- Performance, security, usability, etc. -->
- **Performance:** [Response time, throughput, etc.]
- **Security:** [Authentication, authorization, data protection]
- **Usability:** [User experience requirements]
- **Responsive Design:** Must work on mobile (320px+), tablet (768px+), and desktop (1024px+)
- **Theme Support:** Must support both light and dark mode using existing theme system
- **Compatibility:** [Browser support, device support, etc.]

### Technical Constraints
<!-- What limitations exist? -->
- [Constraint 1: Must use existing X system]
- [Constraint 2: Cannot modify Y database table]
- [Constraint 3: Must be backward compatible with Z]

---

## 6. Data & Database Changes

### Database Schema Changes
<!-- If any database changes are needed -->
```sql
-- Example: New table creation
-- Include all DDL statements, migrations, indexes
```

### Data Model Updates
<!-- Changes to TypeScript types, Drizzle schemas, etc. -->
```typescript
// Example: New types or schema updates.
// When defining Drizzle schemas, consider adding indexes for frequently queried columns.
// e.g. import { index } from "drizzle-orm/pg-core";
//      pgTable(..., (table) => ([ index("name_idx").on(table.name) ]));
```

### Data Migration Plan
<!-- How to handle existing data -->
- [ ] [Migration step 1]
- [ ] [Migration step 2]
- [ ] [Data validation steps]

### 🚨 MANDATORY: Down Migration Safety Protocol
**CRITICAL REQUIREMENT:** Before running ANY database migration, you MUST create the corresponding down migration file following the `drizzle_down_migration.md` template process:

- [ ] **Step 1: Generate Migration** - Run `npm run db:generate` to create the migration file
- [ ] **Step 2: Create Down Migration** - Follow `drizzle_down_migration.md` template to analyze the migration and create the rollback file
- [ ] **Step 3: Create Subdirectory** - Create `drizzle/migrations/[timestamp_name]/` directory  
- [ ] **Step 4: Generate down.sql** - Create the `down.sql` file with safe rollback operations
- [ ] **Step 5: Verify Safety** - Ensure all operations use `IF EXISTS` and include appropriate warnings
- [ ] **Step 6: Apply Migration** - Only after down migration is created, run `npm run db:migrate`

**🛑 NEVER run `npm run db:migrate` without first creating the down migration file!**

---

## 7. API & Backend Changes

### Data Access Pattern - CRITICAL ARCHITECTURE RULES

**🚨 MANDATORY: Follow these rules strictly:**

#### **MUTATIONS (Server Actions)** → `app/actions/[feature].ts`
- [ ] **Server Actions File** - `app/actions/[feature].ts` - ONLY mutations (create, update, delete)
- [ ] Examples: `createUser()`, `updateProfile()`, `deleteConversation()`
- [ ] Must use `'use server'` directive and `revalidatePath()` after mutations
- [ ] **What qualifies as mutations**: POST, PUT, DELETE operations, form submissions, data modifications

#### **QUERIES (Data Fetching)** → Choose based on complexity:

**Simple Queries** → Direct in Server Components
- [ ] **Direct in Page Components** - Simple `await db.select().from(table)` calls
- [ ] Example: `const users = await db.select().from(users).where(eq(users.id, userId))`
- [ ] Use when: Single table, simple WHERE clause, used in only 1-2 places

**Complex Queries** → `lib/[feature].ts`
- [ ] **Query Functions in lib/** - `lib/[feature].ts` for complex/reused queries
- [ ] Example: `lib/history.ts` with `getConversationsGrouped()`
- [ ] Use when: JOINs, aggregations, complex logic, used in 3+ places, needs efficient lookups
- [ ] **What qualifies as complex queries**: Real-time polling, JOIN operations, calculated fields, reusable business logic

#### **API Routes** → `app/api/[endpoint]/route.ts` - **RARELY NEEDED**
🛑 **Only create API routes for these specific cases:**
- [ ] **Webhooks** - Third-party service callbacks (Stripe, external services)
- [ ] **Non-HTML Responses** - File downloads, XML/CSV exports, binary data
- [ ] **External API Proxies** - When you need to hide API keys from client
- [ ] **Public APIs** - When building APIs for external consumption

❌ **DO NOT use API routes for:**
- [ ] ❌ Internal data fetching (use lib/ functions instead)
- [ ] ❌ Real-time polling (use lib/ functions called from client)
- [ ] ❌ Form submissions (use Server Actions instead)
- [ ] ❌ User authentication flows (use Server Actions instead)

#### **PROFESSIONAL NAMING (Directory-Based Separation):**
- `app/actions/[feature].ts` - For mutations only (directory context is clear)
- `lib/[feature].ts` - For complex queries and data fetching
- `app/api/[endpoint]/route.ts` - Only for webhooks, file exports, external APIs
- Example: `app/actions/documents.ts` + `lib/documents.ts` (no API route needed)

#### **DECISION FLOWCHART - "Where should this code go?"**

```
📝 What are you building?
│
├─ 🔄 Modifying data? (POST/PUT/DELETE)
│  └─ ✅ Use Server Actions: `app/actions/[feature].ts`
│
├─ 📊 Fetching data? (GET operations)
│  ├─ Simple query (1 table, basic WHERE)?
│  │  └─ ✅ Direct in Server Component: `await db.select()...`
│  └─ Complex query (JOINs, reused, business logic)?
│     └─ ✅ Use lib function: `lib/[feature].ts`
│
└─ 🌐 External integration?
   ├─ Webhook from 3rd party?
   │  └─ ✅ API Route: `app/api/webhooks/[service]/route.ts`
   ├─ File download/export?
   │  └─ ✅ API Route: `app/api/export/[type]/route.ts`
   └─ Internal app feature?
      └─ ❌ NO API ROUTE! Use Server Actions or lib/ instead
```

### Server Actions
<!-- New or modified server actions for mutations -->
- [ ] **`create[Model]`** - [Description of create operation]
- [ ] **`update[Model]`** - [Description of update operation]  
- [ ] **`delete[Model]`** - [Description of delete operation]

### Database Queries
<!-- How you'll fetch data - be explicit about the choice -->
- [ ] **Direct in Server Components** - Simple queries only (single table, basic WHERE)
- [ ] **Query Functions in lib/queries/** - Complex queries (JOINs, aggregations, reused 3+ times)

### API Routes (Only for Special Cases)
<!-- 🛑 ONLY create API routes when Server Actions and lib/ functions cannot handle the use case -->
- [ ] **Webhooks** - Third-party service callbacks (Stripe, external services)
- [ ] **Non-HTML Responses** - File downloads, XML/CSV exports, binary data  
- [ ] **External API Proxies** - When you need to hide API keys from client
- [ ] **Public APIs** - When building APIs for external consumption

**❌ DO NOT create API routes for internal data operations - use Server Actions (mutations) or lib/ functions (queries) instead**

### External Integrations
<!-- Third-party APIs, services, etc. -->
- [Service 1: Purpose and configuration]
- [Service 2: API keys and setup required]

**🚨 MANDATORY: Use Latest AI Models**
- When using Gemini models, always use **gemini-2.5-flash** (never gemini-1.5 or gemini-2.0 models)
- When using OpenAI models, use **gpt-4o** (never gpt-3.5-turbo as default)

---

## 8. Frontend Changes

### New Components
<!-- Components to create in components/ directory, organized by feature -->
- [ ] **`components/[feature]/ComponentName.tsx`** - [Purpose and props]
- [ ] **`components/[feature]/AnotherComponent.tsx`** - [Functionality description]

**Component Organization Pattern:**
- Use `components/[feature]/` directories for feature-specific components
- Example: `components/chat/`, `components/auth/`, `components/dashboard/`
- Keep shared/reusable components in `components/ui/` (existing pattern)
- Import into pages from the global components directory

**Component Requirements:**
- **Responsive Design:** Use mobile-first approach with Tailwind breakpoints (`sm:`, `md:`, `lg:`)
- **Theme Support:** Use CSS variables for colors, support `dark:` classes for dark mode
- **Accessibility:** Follow WCAG AA guidelines, proper ARIA labels, keyboard navigation

### Page Updates
<!-- Pages that need changes -->
- [ ] **`/path/to/page`** - [What changes are needed]
- [ ] **`/another/page`** - [Modifications required]

### State Management
<!-- How data flows through the app -->
- [Context providers, global state, local state decisions]
- [Data fetching strategies]

---

## 9. Implementation Plan

### Phase 1: Database Changes (If Required)
**Goal:** Prepare and apply database schema changes with safe rollback capability

- [ ] **Task 1.1:** Generate Database Migration
  - Files: `lib/drizzle/schema/*.ts`
  - Details: Update schema files with new fields, tables, or indexes
- [ ] **Task 1.2:** Create Down Migration (MANDATORY)
  - Files: `drizzle/migrations/[timestamp]/down.sql`
  - Details: Follow `drizzle_down_migration.md` template to create safe rollback
- [ ] **Task 1.3:** Apply Migration
  - Command: `npm run db:migrate`
  - Details: Only run after down migration is created and verified

### Phase 2: [Phase Name]
**Goal:** [What this phase accomplishes]

- [ ] **Task 2.1:** [Specific task with file paths]
  - Files: `path/to/file.ts`, `another/file.tsx`
  - Details: [Technical specifics]
- [ ] **Task 2.2:** [Another task]
  - Files: [Affected files]
  - Details: [Implementation notes]

### Phase 3: [Phase Name]
**Goal:** [What this phase accomplishes]

- [ ] **Task 3.1:** [Specific task]
- [ ] **Task 3.2:** [Another task]

### Phase 4: [Phase Name]
**Goal:** [Final integration and testing]

- [ ] **Task 4.1:** [Integration task]
- [ ] **Task 4.2:** [Testing and validation]

...

---

## 10. Task Completion Tracking - MANDATORY WORKFLOW

### Task Completion Tracking - MANDATORY WORKFLOW
🚨 **CRITICAL: Real-time task completion tracking is mandatory**

- [ ] **🗓️ GET TODAY'S DATE FIRST** - Before adding any completion timestamps, use the `time` tool to get the correct current date (fallback to web search if time tool unavailable)
- [ ] **Update task document immediately** after each completed subtask
- [ ] **Mark checkboxes as [x]** with completion timestamp using ACTUAL current date (not assumed date)
- [ ] **Add brief completion notes** (file paths, key changes, etc.) 
- [ ] **This serves multiple purposes:**
  - [ ] **Forces verification** - You must confirm you actually did what you said
  - [ ] **Provides user visibility** - Clear progress tracking throughout implementation
  - [ ] **Prevents skipped steps** - Systematic approach ensures nothing is missed
  - [ ] **Creates audit trail** - Documentation of what was actually completed
  - [ ] **Enables better debugging** - If issues arise, easy to see what was changed

### Example Task Completion Format
```
### Phase 1: Database Cleanup
**Goal:** Remove usage tracking infrastructure and simplify subscription schema

- [x] **Task 1.1:** Create Database Migration for Usage Table Removal ✓ 2025-07-24
  - Files: `drizzle/migrations/0009_flashy_risque.sql` ✓
  - Details: Dropped user_usage table, simplified users subscription_tier enum ✓
- [x] **Task 1.2:** Update Database Schema Files ✓ 2025-07-24  
  - Files: `lib/drizzle/schema/users.ts` (updated enum), `lib/drizzle/schema/ai_models.ts` (removed is_premium_model) ✓
  - Details: Binary free/paid system implemented ✓
- [x] **Task 1.3:** Apply Migration ✓ 2025-07-24
  - Command: `npm run db:migrate` executed successfully ✓
  - Details: Schema changes applied to development database ✓
```

---

## 11. File Structure & Organization

### New Files to Create
```
project-root/
├── app/[route]/
│   ├── page.tsx                      # The route's main UI
│   ├── loading.tsx                   # Instant loading state UI
│   └── error.tsx                     # Route-specific error boundary
├── components/[feature]/
│   ├── FeatureComponent.tsx          # Feature-specific components
│   └── AnotherComponent.tsx
├── app/actions/
│   └── [feature].ts                  # Server actions (mutations only)
└── lib/
    ├── [feature].ts                   # Complex query functions (or lib/queries/[feature].ts)
    └── utility.ts                     # Shared utilities
```

**File Organization Rules:**
- **Components**: Always in `components/[feature]/` directories
- **Pages**: Only `page.tsx`, `layout.tsx`, `loading.tsx`, `error.tsx` in `app/` routes  
- **Server Actions**: In `app/actions/[feature].ts` files (mutations only)
- **Complex Queries**: In `lib/[feature].ts` files (when needed)
- **Utilities**: In `lib/` directory
- **Types**: Co-located with components or in `lib/types.ts`

#### **LIB FILE SERVER/CLIENT SEPARATION - CRITICAL ARCHITECTURE RULE**

**🚨 MANDATORY: Prevent Server/Client Boundary Violations**

When creating lib files, **NEVER mix server-only imports with client-safe utilities** in the same file.

**Server-Only Imports (Cannot be used by client components):**
- `next/headers` (cookies, headers)
- `@/lib/supabase/server` 
- `@/lib/drizzle/db` (database operations)
- Server Actions or other server-side functions
- Node.js modules (fs, path, etc.)

**Decision Flowchart - "Should I split this lib file?"**
```
📁 What's in your lib/[feature].ts file?
│
├─ 🔴 Server-only imports + Client-safe utilities?
│  └─ ✅ SPLIT: Create lib/[feature]-client.ts for client utilities
│
├─ 🟢 Only server-side operations?
│  └─ ✅ KEEP: Single lib/[feature].ts file (server-only)
│
└─ 🟢 Only client-safe utilities?
   └─ ✅ KEEP: Single lib/[feature].ts file (client-safe)
```

**File Naming Pattern:**
- `lib/[feature].ts` - Server-side operations and re-exports
- `lib/[feature]-client.ts` - Client-safe utilities only
- Example: `lib/attachments.ts` + `lib/attachments-client.ts`

### Files to Modify
- [ ] **`existing/file.ts`** - [What changes to make]
- [ ] **`another/file.tsx`** - [Modifications needed]

### Dependencies to Add
```json
{
  "dependencies": {
    "new-package": "^1.0.0"
  },
  "devDependencies": {
    "dev-package": "^2.0.0"
  }
}
```

---

## 12. Error Handling & Edge Cases

### Error Scenarios
- [ ] **Error 1:** [What happens when...] 
  - **Handling:** [How to handle it]
- [ ] **Error 2:** [Another error scenario]
  - **Handling:** [Response strategy]

### Edge Cases
- [ ] **Edge Case 1:** [Unusual scenario]
  - **Solution:** [How to handle]
- [ ] **Edge Case 2:** [Another edge case]
  - **Solution:** [Approach to take]

---

## 13. Security Considerations

### Authentication & Authorization
- [ ] [Who can access this feature?]
- [ ] [What permissions are required?]
- [ ] [How is access controlled?]

### Input Validation
- [ ] [What user inputs need validation?]
- [ ] [What validation rules apply?]
- [ ] [How to prevent injection attacks?]

---

## 14. Deployment & Configuration

### Environment Variables
```bash
# Add these to .env
NEW_API_KEY=your_api_key_here
DATABASE_URL=your_database_url
```

---

## 15. AI Agent Instructions

### Default Workflow - STRATEGIC ANALYSIS FIRST
🎯 **STANDARD OPERATING PROCEDURE:**
When a user requests any new feature, improvement, or significant change, your **DEFAULT BEHAVIOR** should be:

1. **EVALUATE STRATEGIC NEED** - Determine if multiple solutions exist or if it's straightforward
2. **STRATEGIC ANALYSIS** (if needed) - Present solution options with pros/cons and get user direction
3. **CREATE A TASK DOCUMENT** in `ai_docs/` using this template
4. **GET USER APPROVAL** of the task document  
5. **IMPLEMENT THE FEATURE** only after approval

**DO NOT:** Present implementation plans in chat without creating a proper task document first.  
**DO:** Always create comprehensive task documentation that can be referenced later.  
**DO:** Present strategic options when multiple viable approaches exist.

### Communication Preferences
- [ ] Ask for clarification if requirements are unclear
- [ ] Provide regular progress updates
- [ ] Flag any blockers or concerns immediately
- [ ] Suggest improvements or alternatives when appropriate

### Implementation Approach - CRITICAL WORKFLOW
🚨 **MANDATORY: Always follow this exact sequence:**

1. **EVALUATE STRATEGIC NEED FIRST (Required)**
   - [ ] **Assess complexity** - Is this a straightforward change or are there multiple viable approaches?
   - [ ] **Review the criteria** in "Strategic Analysis & Solution Options" section
   - [ ] **Decision point**: Skip to step 3 if straightforward, proceed to step 2 if strategic analysis needed

2. **STRATEGIC ANALYSIS SECOND (If needed)**
   - [ ] **Present solution options** with pros/cons analysis for each approach
   - [ ] **Include implementation complexity, time estimates, and risk levels** for each option
   - [ ] **Provide clear recommendation** with rationale
   - [ ] **Wait for user decision** on preferred approach before proceeding
   - [ ] **Document approved strategy** for inclusion in task document

3. **CREATE TASK DOCUMENT THIRD (Required)**
   - [ ] **Create a new task document** in the `ai_docs/tasks/` directory using this template
   - [ ] **Fill out all sections** with specific details for the requested feature
   - [ ] **Include strategic analysis** (if conducted) in the appropriate section
   - [ ] **🔢 FIND LATEST TASK NUMBER**: Use `list_dir` to examine ai_docs/tasks/ directory and find the highest numbered task file (e.g., if highest is 028, use 029)
   - [ ] **Name the file** using the pattern `XXX_feature_name.md` (where XXX is the next incremental number)
   - [ ] **Present a summary** of the task document to the user for review

4. **GET APPROVAL FOURTH (Required)**
   - [ ] **Wait for explicit user approval** of the task document before writing ANY code
   - [ ] **Ask for feedback and incorporate changes** to the task document if needed
   - [ ] **Update the task document** based on user feedback

5. **IMPLEMENT FIFTH (Only after approval)**
   - [ ] **🚨 CRITICAL: CHECK OFF COMPLETED TASKS IN REAL-TIME**
     - [ ] **Update task document immediately** after completing each task/subtask
     - [ ] **Mark checkboxes as [x]** for completed items
     - [ ] **Add completion notes** with file paths and details when helpful
     - [ ] **This forces verification** that you actually completed what you said you did
     - [ ] **Provides clear progress tracking** for the user to see what's done
   - [ ] Start with Phase 1 and complete fully before moving to Phase 2
   - [ ] **🚨 MANDATORY: For ANY database changes, create down migration file BEFORE running `npm run db:migrate`**
     - [ ] Follow `drizzle_down_migration.md` template process
     - [ ] Create `drizzle/migrations/[timestamp]/down.sql` file
     - [ ] Verify all operations use `IF EXISTS` and include warnings
     - [ ] Only then run `npm run db:migrate`
   - [ ] **For any new page route, create `loading.tsx` and `error.tsx` files alongside `page.tsx`**
   - [ ] Test each component as you build it
   - [ ] Follow existing code patterns and conventions
   - [ ] **Always create components in `components/[feature]/` directories**
   - [ ] Keep pages minimal - only import and use components
   - [ ] **Test all components in both light and dark themes**
   - [ ] **Verify responsive behavior on mobile, tablet, and desktop**
   - [ ] Document any deviations from the approved plan

6. **VERIFY LIB FILE ARCHITECTURE (For any lib/ changes)**
   - [ ] **Audit new lib files** for server/client mixing
   - [ ] **Check import chains** - trace what server dependencies are pulled in
   - [ ] **Test client component imports** - ensure no boundary violations
   - [ ] **Split files if needed** using `[feature]-client.ts` pattern
   - [ ] **Update import statements** in client components to use client-safe files

### What Constitutes "Explicit User Approval"

#### For Strategic Analysis
**✅ STRATEGIC APPROVAL RESPONSES (Proceed to task document creation):**
- "Option 1 looks good"
- "Go with your recommendation"
- "I prefer Option 2"
- "Proceed with [specific option]"
- "That approach works"
- "Yes, use that strategy"

#### For Task Document
**✅ APPROVAL RESPONSES (Start coding immediately):**
- "Proceed"
- "Go ahead"  
- "Approved"
- "Start implementation"
- "Looks good"
- "Begin"
- "Execute the plan"
- "That works"
- "Yes, continue"

**❓ CLARIFICATION NEEDED (Do NOT start coding):**
- Questions about specific implementation details
- Requests for changes or modifications
- "What about..." or "How will you handle..."
- "I'd like to change..."
- "Wait, let me think about..."
- No response or silence

🛑 **NEVER start coding without user approval of the task document first!**  
🛑 **NEVER create task documents without strategic approval (if strategic analysis was conducted)!**  
🛑 **NEVER run `npm run db:migrate` without first creating the down migration file using `drizzle_down_migration.md` template!**

### Code Quality Standards
- [ ] Follow TypeScript best practices
- [ ] Add proper error handling
- [ ] Include comprehensive comments
- [ ] **🚨 MANDATORY: Use early returns to keep code clean and readable**
  - [ ] **Prioritize early returns** over nested if-else statements
  - [ ] **Validate inputs early** and return immediately for invalid cases
  - [ ] **Handle error conditions first** before proceeding with main logic
  - [ ] **Exit early for edge cases** to reduce nesting and improve readability
  - [ ] **Example pattern**: `if (invalid) return error; // main logic here`
- [ ] **🚨 MANDATORY: Use async/await instead of .then() chaining**
  - [ ] **Avoid Promise .then() chains** - use async/await for better readability
  - [ ] **Use try/catch blocks** for error handling instead of .catch() chaining
  - [ ] **Use Promise.all()** for concurrent operations instead of chaining multiple .then()
  - [ ] **Create separate async functions** for complex operations instead of long chains
  - [ ] **Example**: `const result = await operation();` instead of `operation().then(result => ...)`
- [ ] **🚨 MANDATORY: Create down migration files before running ANY database migration**
  - [ ] Follow `drizzle_down_migration.md` template process
  - [ ] Use `IF EXISTS` clauses for safe rollback operations
  - [ ] Include appropriate warnings for data loss risks
- [ ] **Ensure responsive design (mobile-first approach with Tailwind breakpoints)**
- [ ] **Test components in both light and dark mode**
- [ ] **Verify mobile usability on devices 320px width and up**
- [ ] Follow accessibility guidelines (WCAG AA)
- [ ] Use semantic HTML elements
- [ ] **🚨 MANDATORY: Clean up removal artifacts**
  - [ ] **Never leave placeholder comments** like "// No usage tracking needed" or "// Removed for simplicity"
  - [ ] **Delete empty functions/components** completely rather than leaving commented stubs
  - [ ] **Remove unused imports** and dependencies after deletions
  - [ ] **Clean up empty interfaces/types** that no longer serve a purpose
  - [ ] **Remove dead code paths** rather than commenting them out
  - [ ] **If removing code, remove it completely** - don't leave explanatory comments about what was removed

### Architecture Compliance
- [ ] **✅ VERIFY: Used correct data access pattern**
  - [ ] Mutations → Server Actions (`app/actions/[feature].ts`)
  - [ ] Queries → lib functions (`lib/[feature].ts`) for complex, direct in components for simple
  - [ ] API routes → Only for webhooks, file exports, external integrations
- [ ] **🚨 VERIFY: No server/client boundary violations in lib files**
  - [ ] Files with server imports (next/headers, supabase/server, db) don't export client-safe utilities
  - [ ] Client components can import utilities without pulling in server dependencies
  - [ ] Mixed server/client files are split using `-client.ts` pattern
- [ ] **❌ AVOID: Creating unnecessary API routes for internal operations**
- [ ] **❌ AVOID: Mixing server-only imports with client-safe utilities in same file**
- [ ] **🔍 DOUBLE-CHECK: Does this really need an API route or should it be a Server Action/lib function?**
- [ ] **🔍 DOUBLE-CHECK: Can client components safely import from all lib files they need?**

---

## 16. Notes & Additional Context

### Research Links
- [Link to relevant documentation]
- [Reference implementations]
- [Design mockups or wireframes]

### **⚠️ Common Server/Client Boundary Pitfalls to Avoid**

**❌ NEVER DO:**
- Import from `next/headers` in files that export client-safe utilities
- Mix database operations with utility functions in same file
- Import from `@/lib/supabase/server` alongside client-safe functions
- Create utility files that both server and client components import without considering the import chain

**✅ ALWAYS DO:**
- Separate server operations from client utilities into different files
- Use `-client.ts` suffix for client-safe utility files
- Re-export client utilities from main file for backward compatibility
- Test that client components can import utilities without errors

---

## 17. Second-Order Consequences & Impact Analysis

### AI Analysis Instructions
🔍 **MANDATORY: The AI agent must analyze this section thoroughly before implementation**

Before implementing any changes, the AI must systematically analyze potential second-order consequences and alert the user to any significant impacts. This analysis should identify ripple effects that might not be immediately obvious but could cause problems later.

### Impact Assessment Framework

#### 1. **Breaking Changes Analysis**
- [ ] **Existing API Contracts:** Will this change break existing API endpoints or data contracts?
- [ ] **Database Dependencies:** Are there other tables/queries that depend on data structures being modified?
- [ ] **Component Dependencies:** Which other components consume the interfaces/props being changed?
- [ ] **Authentication/Authorization:** Will this change affect existing user permissions or access patterns?

#### 2. **Ripple Effects Assessment**
- [ ] **Data Flow Impact:** How will changes to data models affect downstream consumers?
- [ ] **UI/UX Cascading Effects:** Will component changes require updates to parent/child components?
- [ ] **State Management:** Will new data structures conflict with existing state management patterns?
- [ ] **Routing Dependencies:** Are there route dependencies that could be affected by page structure changes?

#### 3. **Performance Implications**
- [ ] **Database Query Impact:** Will new queries or schema changes affect existing query performance?
- [ ] **Bundle Size:** Are new dependencies significantly increasing the client-side bundle?
- [ ] **Server Load:** Will new endpoints or operations increase server resource usage?
- [ ] **Caching Strategy:** Do changes invalidate existing caching mechanisms?

#### 4. **Security Considerations**
- [ ] **Attack Surface:** Does this change introduce new potential security vulnerabilities?
- [ ] **Data Exposure:** Are there risks of inadvertently exposing sensitive data?
- [ ] **Permission Escalation:** Could new features accidentally bypass existing authorization checks?
- [ ] **Input Validation:** Are all new data entry points properly validated?

#### 5. **User Experience Impacts**
- [ ] **Workflow Disruption:** Will changes to familiar interfaces confuse existing users?
- [ ] **Data Migration:** Do users need to take action to migrate existing data?
- [ ] **Feature Deprecation:** Are any existing features being removed or significantly changed?
- [ ] **Learning Curve:** Will new features require additional user training or documentation?

#### 6. **Maintenance Burden**
- [ ] **Code Complexity:** Are we introducing patterns that will be harder to maintain?
- [ ] **Dependencies:** Are new third-party dependencies reliable and well-maintained?
- [ ] **Testing Overhead:** Will this change require significant additional test coverage?
- [ ] **Documentation:** What new documentation will be required for maintainers?

### Critical Issues Identification

#### 🚨 **RED FLAGS - Alert User Immediately**
These issues must be brought to the user's attention before implementation:
- [ ] **Database Migration Required:** Changes that require data migration in production
- [ ] **Breaking API Changes:** Modifications that will break existing integrations
- [ ] **Performance Degradation:** Changes likely to significantly impact application speed
- [ ] **Security Vulnerabilities:** New attack vectors or data exposure risks
- [ ] **User Data Loss:** Risk of losing or corrupting existing user data

#### ⚠️ **YELLOW FLAGS - Discuss with User**
These issues should be discussed but may not block implementation:
- [ ] **Increased Complexity:** Changes that make the codebase harder to understand
- [ ] **New Dependencies:** Additional third-party packages that increase bundle size
- [ ] **UI/UX Changes:** Modifications that change familiar user workflows
- [ ] **Maintenance Overhead:** Features that will require ongoing maintenance attention

### Mitigation Strategies

#### Database Changes
- [ ] **Backup Strategy:** Ensure database backups before schema changes
- [ ] **Rollback Plan:** Define clear rollback procedures for database migrations
- [ ] **Staging Testing:** Test all database changes in staging environment first
- [ ] **Gradual Migration:** Plan for gradual data migration if needed

#### API Changes
- [ ] **Versioning Strategy:** Use API versioning to maintain backward compatibility
- [ ] **Deprecation Timeline:** Provide clear timeline for deprecated features
- [ ] **Client Communication:** Notify API consumers of breaking changes in advance
- [ ] **Graceful Degradation:** Ensure old clients can still function during transition

#### UI/UX Changes
- [ ] **Feature Flags:** Use feature flags to gradually roll out UI changes
- [ ] **User Communication:** Notify users of interface changes through appropriate channels
- [ ] **Help Documentation:** Update help documentation before releasing changes
- [ ] **Feedback Collection:** Plan for collecting user feedback on changes

### AI Agent Checklist

Before presenting the task document to the user, the AI agent must:
- [ ] **Complete Impact Analysis:** Fill out all sections of the impact assessment
- [ ] **Identify Critical Issues:** Flag any red or yellow flag items
- [ ] **Propose Mitigation:** Suggest specific mitigation strategies for identified risks
- [ ] **Alert User:** Clearly communicate any significant second-order impacts
- [ ] **Recommend Alternatives:** If high-risk impacts are identified, suggest alternative approaches

### Example Analysis Template

```
🔍 **SECOND-ORDER IMPACT ANALYSIS:**

**Breaking Changes Identified:**
- Database schema change will require migration of 10,000+ existing records
- API endpoint `/api/users` response format changing (affects mobile app)

**Performance Implications:**
- New JOIN query may slow down dashboard load time by 200ms
- Additional React components will increase bundle size by 15KB

**Security Considerations:**
- New user input field requires XSS protection
- API endpoint needs rate limiting to prevent abuse

**User Experience Impacts:**
- Navigation menu restructure may confuse existing users
- New required field will interrupt existing signup flow

**Mitigation Recommendations:**
- Implement database migration script with rollback capability
- Use API versioning to maintain backward compatibility
- Add performance monitoring for new queries
- Plan user communication strategy for UI changes

**🚨 USER ATTENTION REQUIRED:**
The database migration will require approximately 30 minutes of downtime. Please confirm if this is acceptable for your deployment schedule.
```

---

*Template Version: 1.2*  
*Last Updated: 7/24/2025*  
*Created By: Brandon Hancock*
