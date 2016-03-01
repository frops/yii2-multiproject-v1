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
		project1 /
			views /
				layouts /
					main.php
			assets /
				AppAsset.php extends application/common/assets/AppAsset.php
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
				project1 / 
					assets /
						NewsAssets.php extends application/modules/news/common/assets/NewsAsset.php
					models / 
						Category.php extends application/modules/news/common/models/Category.php
						News.php extends application/modules/news/common/models/News.php
					static / 
						css /
							news.css