This is surprisingly tricky. Right now, for trait calls we obtain the trait reference without associated types from rustc, which is why we reference the type class argument by assoc-types-excluding name instead of by full type. But names obviously don't know anything about subtyping.