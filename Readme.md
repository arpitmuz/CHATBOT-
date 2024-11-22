step-1 create a new folder and open vs code  in it and open terminal and write
conda create -v venv python==3.10 -y
pip install virtualenv
python -m venv myenv
.\myenv\Scripts\Activate.ps1
second-option=create virtual environment using pi

step 2: create a requirements.txt file
streamlit
python-dotenv
google-generativeai

Now open the terminal and write
pip install -r requirements.txt

Now we will create '.env' file in which we store our secrets
secrets.
Go to Browser and write Makersuite Apikeys --> Create a api key -> copy it and paste it in.env file
GOOGLE_API_KEY="PASTE YOUR API KEY"


step 4: WE WILL CREATE 'APP.PY' FILE WHERE WE WILL CREATE A FUNCTION THAT WILL TAKE OUR QUERY AS AN ARGUMENT AND SEND IT TO GOOGLE_GENERATIVE_MODEL AND OUR GENERAVTIVE MODEL WILL RESPONSE BASED ON YOUR QUERY IN TEXTUAL FORMAT.HERE WE WILL USE STREAMLIT FOR OUR PAGE_TITLE DESDIGN,INPUT_FIELD_DESIGN.when user click to submit button then our function will run and return our response

open the terminal and write
streamlit run app.py

step5:go to github and create a nwe repository and fill repository name and write commands on terminal of our vascode
git init 
git add .
git commit -m "first commit"
git branch -M main
git remote add origin  https://github.com/arpitmuz/CHATBOT-.git
git push -u origin main



step-6: create a .git ignore file and myvenv/and .env file .put all files and folder which you dont want to push on github

step 7: go to browser --> streamlit cloud -> register your account --> 
create app --> deploy public app -> 
step 6:' fill the project repository name
in secrets-> paste all secret present in .env file