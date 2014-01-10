django-group-user-mngt
======================

settings.py
-----------
Add to INSTALLED_APPS : 'group_user_mngt',

GROUP_MANAGEMENT_TEMPLATE = 'manage_groups.html'

urls.py
-------

url(r'^groupmanagement/', include('group_user_mngt.urls', namespace="gm_space")),

Under static root :

mkdir group_user_mngt 
cd group_user_mngt 
cp -r /usr/local/lib/python2.7/dist-packages/group_user_mngt/static/group_user_mngt/* .

Group view 
----------
http://<FQDN>/groupmanagement/group/update/
