# COMMENTATOR

- A Code-mixed Multilingual Text Annotation Framework.
- Code-mixing on Hinglish Data.
- Easy extensibility to other code-mixed language pairs such as Gujarati-English, Marathi-English etc.

### 1. Folder Structure :books:

```
backend
	app.py
	requirements.txt
	Dockerfile
	LID_tool
fronend
	build
	node_module
	public
	src
		Admin
		Auth
		Components
		Edit
		Home
		User
		utils
		Router.js
	.env
	.ignore
	package-lock.json
	package.json
```

##### frontend/src/.env

    REACT_APP_BACKEND_URL=http://<YOUR_BACKEND_IP_ADDRESS>:5000
    OR
    REACT_APP_BACKEND_URL=http://localhost:5000

---

### 2. Database Schemas :department_store:

|           |                                             |
| --------- | ------------------------------------------- |
| lid       | LID based Language Identification of Tokens |
| sentences | Sentences to be annotated                   |
| users     | Admin & Annotator Accounts                  |

### 3. Backend [ Local Server ] :computer:

##### Steps to Follow

a. Navigate inside backend folder

    cd backend

b. Installing Dependencies

    pip install -r requirements.txt

c. Updating Frontend URL

> Open `app.py` in a code/text editor (Visual Studio Code, Sublime Text, Notepad etc)

    frontend = YOUR_FRONTEND_HOST_URL
    OR
    frontend = http://localhost:3000

d. Updating MongoDB URL

> Open `app.py` in a code/text editor (Visual Studio Code, Sublime Text, Notepad etc)

    conn_str = YOUR_MONGODB_URL

e. Download LID Code from the google drive link attached above

> Navigate to Drive > Downloads > LID & download the zip file
>
> Extract zip file in LID_tool folder

f. Running the local server

    python app.py
    OR
    py app.py

---

### 4. Frontend [ Local Server ] :computer:

##### Steps to Follow

a. Navigate inside backend folder

    cd frontend

b. Install all frontend dependencies post 1st application download.
npm i

c. Start the frontend local server.

    npm start

> OR click on the frontend bash/shell file to run the frontend local server.

---

### 5. Administrative Configuration :passport_control:

##### Steps to Follow

1. Start Frontend and Backend Local Server. (Refer 2.e & 3.c)
2. Create an admin account.
3. Open MongoDB database and set `admin=True` to create superuser/admin account.
4. Login to Admin Dashboard.
5. Upload sentences to the database (csv).

