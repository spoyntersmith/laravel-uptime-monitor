node {
   // Mark the code checkout 'stage'....
   stage 'Checkout'
   echo 'Fetching...'

   // Get some code from a Bitbucket repository
   checkout scm
   // Install dependencies
   stage 'Install dependencies'
   // Run Composer
   sh 'composer install'
   // Test stage
   stage 'Test'
   // Run the tests
   sh "vendor/bin/phpunit"
}
