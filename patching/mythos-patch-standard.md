# Mythos Patch Instructions (Canonical)

All patches must be in the `#FILE:` block format with matching `#END` tags.  
Patches must always be based on the current GitHub repo state.

## ✅ Example
```diff
#FILE: praetorian_server/routes/__init__.py
@@ -1 +1,3 @@
 # Namespace package for routes shims
+
+from .apply_patch_dev import apply_patch_dev_router
#END
```

## ❌ Forbidden
- No `diff --git`, `index`, `---`, or `+++`
- No missing `#END`
- No guesswork
