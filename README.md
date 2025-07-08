# General Code Order

✅ **1. Imports**  
   Always import in this clear order:  
   - **Libraries:** React, Next.js, third-party packages  
     _(e.g., `import React from "react";` · `import Link from "next/link";`)_
   - **Custom Hooks:** project-specific hooks  
     _(e.g., `import { useAuth } from "@/hooks/useAuth";`)_
   - **Types:** TypeScript types  
     _(e.g., `import type { User } from "@/types/user";`)_
   - **Components:** local UI components  
     _(e.g., `import Header from "@/components/Header";`)_
   - **Utils:** generic helpers  
     _(e.g., `import { formatDate } from "@/utils/date";`)_

---

✅ **2. Setup**  
   Always declare in this clear order:  
   - **Router:** Next router  
     _(e.g., `const router = useRouter();`)_
   - **Translations:** i18n or language hook  
     _(e.g., `const t = useTranslations("Common");`)_
   - **Queries:** read data  
     _(e.g., `const { data } = useFetchData();`)_
   - **Mutations:** write or update data  
     _(e.g., `const { mutate } = usePostData();`)_

---

✅ **3. State**  
   - `useState` declarations  
     _(e.g., `const [count, setCount] = useState(0);`)_

✅ **4. Effects**  
   - `useEffect` for side effects  
     _(e.g., `useEffect(() => { ... }, []);`)_

✅ **5. Action Functions**  
   - Pure helper logic inside the component  
     _(e.g., `function calculateTotal() { ... }`)_

✅ **6. Handler Functions**  
   - Event handlers, API calls, user actions  
     _(e.g., `function handleSubmit() { ... }`)_

✅ **7. Loading**  
   - Show loader if needed  
     _(e.g., `if (isLoading) return <Spinner />;`)_

✅ **8. Return JSX**  
   - Render the UI  
     _(e.g., `return <div>Hello World</div>;`)_

✅ **9. Export**  
   - Export the component  
     _(e.g., `export default ExampleComponent;`)_

---

✅ **Tip:** Use this exact order for clean, consistent, easy-to-read files!
