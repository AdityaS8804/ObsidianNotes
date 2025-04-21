	server {
	    listen 8000;
	    server_name 127.0.0.1;
	    #Auth-Service
	    location /api/v1/auth/ {
		proxy_pass http://127.0.0.1:5001;
		proxy_set_header Host $host;
		proxy_set_header X-Real-IP $remote_addr;
	    }



	    #Chat service
	    location /api/v1/chat/ {
		proxy_pass http://127.0.0.1:5002;
		proxy_set_header Host $host;
		proxy_set_header X-Real-IP $remote_addr;

		proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for;

	}


		#Graph-Service
		location /api/v1/graph/ {
		proxy_pass http://127.0.0.1:5003;
		proxy_set_header Host $host;
		proxy_set_header X-Real-IP $remote_addr;
		}

	    location / {
		return 404;
	    }
	}
