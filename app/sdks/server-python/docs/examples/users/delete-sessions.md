from appwrite.client import Client
from appwrite.services.users import Users

client = Client()

(client
  .set_project('5df5acd0d48c2') # Your project ID
  .set_key('919c2d18fb5d4...a2ae413da83346ad2') # Your secret API key
)

users = Users(client)

result = users.delete_sessions('[USER_ID]')