# MyAngularProject


# Installing CodeDeploy Agent
sudo yum update -y<br>
sudo yum install -y ruby wget<br>
wget https://aws-codedeploy-eu-west-1.s3.eu-west-1.amazonaws.com/latest/install<br>
chmod +x ./install<br>
sudo ./install auto<br>

# Checking CodeDeploy Agent status
sudo service codedeploy-agent status<br>
sudo service codedeploy-agent start

# Installing Nginx
sudo amazon-linux-extras install -y nginx1

# Checking Nginx status
sudo service nginx status

# Starting Nginx
sudo service nginx start

# Enabling Nginx to restart on system reboot
sudo chkconfig nginx on

# Creating folders for deployments
sudo mkdir -p /var/www/my-angular-project

# Changing Nginx configuration
sudo nano /etc/nginx/nginx.conf

# Only change root to /var/www/my-angular-project
# Press `Ctrl + X` to exit, press `Y` to save and press `Enter` to approve.

# Restart Nginx
sudo service nginx restart




This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 9.0.6.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `--prod` flag for a production build.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI README](https://github.com/angular/angular-cli/blob/master/README.md).
