# Set utp railway 

# generate djagno keys
python manage.py shell -c 'from django.core.management import utils; print(utils.get_random_secret_key())'

# deploy django + postgres + celery + redis project template on railway

# set up locally
scoop bucket add railway https://github.com/railwayapp/scoop-railway; scoop install railway/railway

railway link <project-id-kind of number>

# to deploy
railway up







git remote set-url origin https://git-repo/new-repository.git
