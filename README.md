# Пример структуры мультипроектного сайта на Yii2 
#### Структура

	application /
		common /
			controllers /
				BaseController.php
			assets /
				AppAsset.php				
			static / 
				js /
					main / 
						main.js
				css / 
					main / 
						main.css
		wf /
			views /
				layouts /
					main.php
			assets /
				AppAsset.php extends app/common/assets/AppAsset.php
			static /
				js / 
					main/
						main.js	
				css /
					main /
						main.css	
		modules / 
			news /
				common /
					assets /
						NewsAssets.php
					models /
						Category.php
						News.php
					controllers /
						DefaultController.php
					static / 
						css /
							news.css
						js / 
							news.js
				wf / 
					assets /
						NewsAssets.php extends app/modules/news/common/assets/NewsAsset.php
					models / 
						Category.php extends app/modules/news/common/models/Category.php
						News.php extends app/modules/news/common/models/News.php
					static / 
						css /
							news.css