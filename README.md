# General Code Order

✅ **1. Imports**  
   Always import in this clear order:  
   - **Libraries:** React, Next.js, built-in hooks  
     _(e.g., `import React, { useState } from "react";` · `import Link from "next/link";`)_
   - **Custom Hooks & Lib:** project logic, hooks, API calls  
     _(e.g., `import { useGetProfile } from "@/lib/hooks";`)_
   - **Types:** TypeScript types  
     _(e.g., `import type { User } from "@/types/user";`)_
   - **Components:** local UI components  
     _(e.g., `import Navbar from "@/components/Navbar";`)_
   - **Utilities:** generic helpers  
     _(e.g., `import { formatDate } from "@/utils/formatDate";`)_

---

✅ **2. Setup**  
   - Router, translations, queries, mutations  
     _(e.g., `const router = useRouter();`)_

✅ **3. State**  
   - `useState` declarations  
     _(e.g., `const [data, setData] = useState();`)_

✅ **4. Effects**  
   - `useEffect` for side effects

✅ **5. Action Functions**  
   - Pure helpers/utilities inside the component  
     _(e.g., `getName()`)_

✅ **6. Handler Functions**  
   - Trigger actions, API calls, mutations  
     _(e.g., `handleClick()`, `handleSubmit()`)_

✅ **7. Loading**  
   - Show loader if needed  
     _(e.g., `if (isLoading) return <Loading />;`)_

✅ **8. Return JSX**  
   - Render the UI  
     _(inside `return (...)`)_

✅ **9. Export**  
   - Export the component  
     _(e.g., `export default MyComponent;`)_

---

✅ **Tip:** Use this order in every file for clear, maintainable code!
