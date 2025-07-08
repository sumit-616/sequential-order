# General Code Order

✅ **1. Imports**  
   Always import in this clear order:  
   - **Libraries:** React, Next.js, built-in hooks  
     _(e.g., `import React, { useState } from "react";` · `import Link from "next/link";`)_
   - **Custom Hooks:** project-specific hooks  
     _(e.g., `import { useGetProfile } from "@/lib/hooks";`)_
   - **Types:** TypeScript types  
     _(e.g., `import type { User } from "@/types/user";`)_
   - **Components:** local UI components  
     _(e.g., `import Navbar from "@/components/Navbar";`)_
   - **Utils:** generic helpers  
     _(e.g., `import { formatDate } from "@/utils/formatDate";`)_

---

✅ **2. Setup**  
   Always declare in this clear order:  
   - **Router:** Next router  
     _(e.g., `const router = useRouter();`)_
   - **Translations:** i18n translations  
     _(e.g., `const t = useTranslations("Dashboard");`)_
   - **Queries:** data fetching hooks  
     _(e.g., `const { data } = useGetProfile();`)_
   - **Mutations:** actions for POST, PUT, DELETE  
     _(e.g., `const { mutate } = useSendConnectionRequest();`)_

---

✅ **3. State**  
   - `useState` declarations  
     _(e.g., `const [data, setData] = useState();`)_

✅ **4. Effects**  
   - `useEffect` for side effects

✅ **5. Action Functions**  
   - Pure helper logic inside the component  
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

✅ **Tip:** Use this order exactly for clear, maintainable code!
