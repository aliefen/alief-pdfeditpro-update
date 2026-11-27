# alief-pdfeditpro-update

Automatic updates for **ALIEF PDF EDITOR PRO** (PT. ALIEF ENERGY UTAMA, Batam).

* `alief_pdfeditpro_update.json` – signed release notice (Ed25519) read by the installed program at start-up and every 4 hours
* `app-<version>.zip` – update package, verified with SHA-256 before it is used
* `qtgl-<pyside version>.zip` – Qt OpenGL components for the 3D review (shared by later updates, downloaded once)

The program downloads new versions in the background to `%LOCALAPPDATA%\AliefEnergy\ALIEF_PDFEDITPRO\app\<version>`
(no administrator rights needed) and shows a notification. Packages without a valid signature are ignored.
