# FirstDjangoProject
Designed a Shopping website using django

## Steps to create a django project
<ol>
  <li>Install Django <br><code>pip install django</code></li>
  <li>Create a Django Project <br>
    <code>django-admin startproject shop .</code>
  </li>
  <li>Run Development server<br>
    <code> python manage.py runserver</code>
  </li>
  <li>Create a application<br>
    <code> python manage.py startapp Products</code>
  </li>
  <li>Create a view functions and link with the url
    <ul>
      <li>write a view in views.py</li>
      <li>Create a urls.py file in Products folder</li>
      <li>Write a urlpatterns list and add mapping of view fuction with the url</li>
      <li>Add the url mapping in main project urls.py file</li>
    </ul>
  </li>
  <li>Creating a Product Class in models.py</li>
  <li>Storing the database in sqlite<br>
    <ul>
      <li>Update settings.py, in INSTALLED_APPS list add 'Products.apps.ProductsConfig'</li>
      <li>Update the sqlite database<br>
      <code>python manage.py makemigrations</code><br>
      <code>python manage.py migrate</code>
      </li>
    </ul>
  </li>
  <li>Manage Admin Panel
  <ul>
    <li> Create superuser <br>
      <code> python manage.py createsuperuser</code>
    </li>
    <li>Add Product management in Admin Panel<br>
      <ul>
        <li>Register the product class in admin.py<br> 
          <code> admin.site.register(Product)</code>
          </li>
        <li>Changing the display list <br>
          <code>Create ProductAdmin class in admin.py and add fields in list_dispaly </code>
        </li>
      </ul>
    </li>
  </ul>
  </li>
</ol>
