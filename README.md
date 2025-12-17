# Malicious-Data-Detector
malicious data detector
elif select == 4:
exit()
else:
print("Invalid choice. Exiting...") time.sleep(3) exit(
Start the program
start()
print("Bad input\nExiting...") time.sleep(3)
exit()
else:
1f choice.lower()- 'y':
start()
elif choice.lower() =m 'n':
exit()
elif select ." 3:
run_URL()
choice = input("Do you want to search again? (y/n)") if choice.lower() not in ['y', 'n'): print("Bad input\nExiting...") time.sleep(3) exit()
else:
1f choice.lower() " 'y':
start()
elif choice.lower() "= `n':
exit(
choice = input("Do you want to search again? (y/n)")
if choice.lower() not in ['y', 'n"]: print("Bad input\nExiting...") time.sleep(3) exit()
else:
if choice.lower() == 'y': start () elif choicolower() =m 'n': exit()
elif select == 2:
f Get user input for cmai]
user_input = input("Enter data to check for malicious content: ") if is malicious data(user input):
print("Potentially malicious data detected.")
else:
print("No malicious data found.")
choice - input("Do you want to scarch again? (y/n)") if choice.lower() not in f'v'. 'n'1:
def start():
print(pyfiglet.figlet_format("Malware Detector using ML")) print(" Welcome to antimalware detector In")
print(" 1. Email scanner") print(" 2. malware scanner") print(" 3. url scanner") print("4. Exitin")
select = int(input("Enter your choice :"))
if select in [1, 2, 3): if select a= 1:
# Get user input for emall
email- input("Enter your email:\n") 1f is_suspicious_email(email):
print("Suspicious email detected!, be aware of this emall")
else:
print("Ema1l is not suspiclous you can work on it.")
choice = input("Do you want to search again? (y/n)")
 malicious_patterns = I
r`\b(attack|ealware|virus|exploit|suspecious|phisinglaccess|delete|chan; r'Ib\d(3)-\d(2)-\d(4)\b'# Example: Social Security Number
for pattern in malicinis_patterns: if re.search(pattern, input_string, re.IGNORECASE): return True
return false
Comment Code
def run_URL():
os.systen("python3 Extract/url_main.py')
Comment Code
def exit():
os.systen(exit')
Comment Code
inport os
import re
import time
import pyfiglet
Define a regular expression pattern to detect suspicious email addresses email_pattern = r'^[a-zA-20-9._X+-]+@[a-zA-20-9.-]+I.[a-zA-2) (2,4)$"
Function to check if the provided email is suspiclous Comment Code
def is_suspicious_email(emall): if re.match(email_pattern, email): return False else: return True
Comment Code
def is_malicious_data(input_string): Define patterns for potentially malicious data malicious_patterns = [
 f1.close() file . "Classifler/pickel vector.pkl" with open(flle, 'rb') as f2: vectorizer pickle. d(f2) f2.close() #predicting X= vectorizer.transform(s_url) y_predict = lgr.predict(x) for site in whitelist: s_url.append(site) sprint(s_url) predict - l1st(y_predict) for j in range(0,len(whitelist)): predict.append(good") print("InThe entered domain is: ", predict[0]) print("In\nIf you feel that this prediction is wrong, \n or if you are not so su
raw2 S str(rawl[j]).split(".") slash_token = slash_token + raw2 dot_token_slash - dot_token_slash + rawl + slash_token token = list(set(dot_token_slash)) if 'com' in token: token.remove(*com") return token
urls= [) urls.append(input("Input the URL that you want to check (eg. google.com) :")) eprint (urls)
Using whitelist filter as the model fails in many legit cases since the bigge whitelist - ['hackthebox.eu','root-me.org','gmail.com*] s_url - [1 for 1 in urls if 1 not in whitelist)
sloading the mode) file = "Classifier/pickel_model.pkl" with open(file, 'rb') as fl: lgr---pickle.load(f1)
import pickle
import random
import numpy as np
import pandas as p
from sklearn.feature extraction.text import TfidfVectorizer from sklearn.linear_model import LogisticRegression from sklearn.model_selection import train_test_split
def sanitization(web):
web- web.lower () token= [] dot_token_slash = [ raw_slash = str(web).split("/") for 1 in raw_slash: raw1 = str(i).split("-") slash_token - ] for j in range(0,len(raw1)): raw2 str(raw1[j]).split(".')
