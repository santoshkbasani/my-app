node{
   stage('SCM Checkout'){
     git 'https://github.com/javahometech/my-app'
   }
   stage('Compile-Package'){
    sh 'mvn clean package'
	}
   stage('Email Notification'){
	   mail bcc: '', body: '''Hi Welcome to Jenkins email alerts.

	   Thanks,
 	   SantoshBasani.''', cc: '', from: '', replyTo: '', subject: 'Jenkins Job', to: 'santoshbasani@gmail.com'
   }
}
