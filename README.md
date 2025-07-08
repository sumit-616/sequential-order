# General Code Order

✅ **1. Imports**  
   Always import in this clear order:  
   - **Libraries:** React, Next.js, built-in hooks  
     _(e.g., `import React, { useState } from "react";` · `import Link from "next/link";`)_
   - **Custom Hooks:** project-specific hooks  
     _(e.g., `import { useGetProfile } from "@/lib/hooks";`)_
   - **Types:** TypeScript types  
     _(e.g., `import type { User } from "@/types/user";`)_
   - **Components & Utilities:** local UI, helpers, utilities  
     _(e.g., `import Navbar from "@/components/Navbar";` · `import { toast } from "@/components/ui/use-toast";`)_

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
   - Pure helpers/utilities  
     _(e.g., `getName()`)_

✅ **6. Handler Functions**  
   - For actions, API calls, mutations  
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

✅ **Tip:** Keep this order consistent in every file for clear, maintainable code!
