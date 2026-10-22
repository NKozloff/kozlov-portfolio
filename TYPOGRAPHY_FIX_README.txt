FIX FOR HEADING FONTS

The typography CSS rules for old headings have not been changed.
The previous full ZIP omitted five original font files.
The CSS in this ZIP now tries local font files in assets/ first and falls back to the same files in the public NKozloff/kozlov-portfolio GitHub repository.

IMPORTANT: Keep your existing original font files in assets/ when replacing site content. This archive does not contain those binary font files. For a fully self-contained offline site, restore your original assets/ fonts from your own earlier website backup.

Upload all the files and folders in this ZIP into the root of your GitHub repository. Keep any existing assets files not included in this archive.

Ensure that root stylesheet is named styles.css (with an s at the end of 'styles'). This is what the HTML references.

If fonts look unchanged immediately, clear cache (Cmd + Shift + R).
