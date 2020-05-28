import os
from flask import Flask ,render_template, request 

app = Flask(__name__) 

@app.route("/")
def index(): 
	return	render_template("index.html")

@app.route("/Partner-Opt-Out/")
def popt(): 
	return	render_template("popt.html")
 
 
@app.route("/Privacy-Policy/")
def pp(): 
	return	render_template("pp.html")

@app.route("/Terms-Of-Services/")
def tos(): 
	return	render_template("tos.html")
  
