# Afrirent

Plateforme immobilière : API Django (`Backend/`) et interface React + Vite (`Frontend/`).

<!-- nouveau-pc:debut -->
## Installer sur un nouveau PC

**Prérequis :** Git, Python 3.12, Node.js 20 ou plus et PostgreSQL.

```bash
git clone git@github.com:Magloireaffokpe/Afrirent.git
cd Afrirent/Backend
python3 -m venv env_afri
source env_afri/bin/activate   # Windows : env_afri\Scripts\activate
pip install -r requirements.txt
cp .env.example .env         # puis remplir les valeurs (DB_*, SECRET_KEY, CLOUDINARY_*)
python manage.py migrate
python manage.py runserver

# Dans un autre terminal
cd Frontend
npm install
cp .env.example .env
npm run dev
```

Créer au préalable une base PostgreSQL correspondant à `DB_NAME`, `DB_USER` et `DB_PASSWORD`.

**À recopier à la main (hors Git) :** `Backend/.env`.
<!-- nouveau-pc:fin -->
