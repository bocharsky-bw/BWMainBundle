BWMainBundle
============

The basic structure of the application, which includes the main templates and functionality

Installing
----------

1. Create ```src\BW\MainBundle``` directory and copy the files of this repository

2. Register the bundle in you ```AppKernel``` in the main section

        // app/AppKernel.php
        public function registerBundles()
        {
            $bundles = array(
                // other bundles here...
                new BW\MainBundle\BWMainBundle(),
            );

            // other code here...

            return $bundles;
        }

3. Add the following route to your routing configuration

        #app/config/routing.yml
        bw_main:
            resource: "@BWMainBundle/Resources/config/routing.yml"
            prefix:   /
