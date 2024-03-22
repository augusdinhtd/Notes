App Password: 
automationtest-1: ATBBAK92CEd37CgsGkHnwkJ7SQWrFDF13DE2


URL_API_BACKEND=https://api-realauth.poeta-internal.com

URL_WEB=https://realauth.poeta-internal.com

# URL_API_BACKEND=http://realauth-api.local/api

# URL_WEB=http://realauth-api.local

#URL_WEB=https://realauthentication.poeta-internal.com

  

BROWSER_DRIVER=/home/dinhtran/RA/chromedriver_linux64/chromedriver

ACCESS_TOKEN=z8xl7K5C42oJZ5p3WMzlVxkRNUILOXGBiMBp263x5j2zdlgJedp4ihOza9xr

ASSETS_IMAGE_URL='/assets/images/'

  

CLIENT_ID=1

CLIENT_SECRET=jbHh0Fdq1VDIwLO0yGRD8UjjtgaCO18QBp9dreCP



//5904672 local 5911579




-----------------
// Temporary v2 routes

Route::domain(config('app.public_customer_api_domain'))->prefix('v2')

->middleware($middleware)

->group(base_path('routes/api.v1.public.php'));

Route::domain(config('app.public_api_domain'))->prefix('api/v2')

->middleware($middleware)

->group(base_path('routes/api.v1.public.php'));