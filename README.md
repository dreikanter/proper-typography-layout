# Proper English and Russian Typography Layout for macOS

## Installation

1. Switch to a built-in layout (such as ABC).
2. Remove unwanted layouts in System Settings → Keyboard → Text Input → Edit.
3. Manually delete their bundles from `/Library/Keyboard Layouts/` and
   `~/Library/Keyboard Layouts/`, if present:

   ```sh
   sudo rm -r '/Library/Keyboard Layouts/[Unwanted Layout].bundle'
   rm -r "$HOME/Library/Keyboard Layouts/[Unwanted Layout].bundle"
   ```

4. Clone the repository and install the bundle:

   ```sh
   git clone https://github.com/dreikanter/proper-typography-layout.git
   cd proper-typography-layout
   sudo cp -R ./ProperTypographyLayout.bundle '/Library/Keyboard Layouts/'
   ```

5. Log out and log back in.
6. Go to System Settings → Keyboard → Text Input → Edit, click + and add **English – Proper Typography** and/or **Russian – Proper Typography**.
7. Select the new layout and test the grave/tilde key.
