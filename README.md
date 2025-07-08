# General Code Order

✅ **1. Imports** — Always import in this order for clarity:

   1️⃣ **Libraries** — React, Next.js, built-in hooks  
   _(e.g., `import React, { useState } from "react";` → `import Link from "next/link";`)_

   2️⃣ **Custom Hooks** — your project’s custom hooks  
   _(e.g., `import { useGetProfile } from "@/lib/hooks";`)_

   3️⃣ **Types** — TypeScript types  
   _(e.g., `import type { User } from "@/types/user";`)_

   4️⃣ **Components & Utilities** — local UI components, helper modules, utilities  
   _(e.g., `import Navbar from "@/components/Navbar";` → `import { toast } from "@/components/ui/use-toast";`)_

✅ **2. Setup** — router, translations, queries, mutations

✅ **3. State** — `useState`

✅ **4. Effects** — `useEffect`

✅ **5. Action Functions** — pure helper or utility functions _(e.g., `getName`)_

✅ **6. Handler Functions** — trigger actions or API calls _(e.g., `handleClick`, `handleSubmit`)_

✅ **7. Loading** — show loader if needed

✅ **8. Return JSX** — render UI

✅ **9. Export** — export the component

Keep every file clear and consistent.
