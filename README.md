#node-mongo-seeds 
[![Build Status](https://travis-ci.org/toymachiner62/node-mongo-seeds.svg?branch=master)](https://travis-ci.org/toymachiner62/node-mongo-seeds)
[![Code Climate](https://codeclimate.com/github/toymachiner62/node-mongo-seeds/badges/gpa.svg)](https://codeclimate.com/github/toymachiner62/node-mongo-seeds)

A tool to quickly populate your mongo db from a set of .json files. The concept is very similar to Ruby on Rails idea of seeding a database. This allows a new developer to pull down the source code for a project (which contains .json files to populate their mongodb with) and run a command and bingo!! database populated and ready to rock.

## Usage

- Run `$ npm install -g node-mongo-seeds`
- Run `$ setup`
- Replace `"localhost/CHANGE_ME_TO_YOUR_DB_NAME"` with the path to your mongodb in your brand new seed.json file
- Create a `/seeds` folder in your project root and put `.json` files in there.
		The name of the file is going to be the collection name in mongo and the contents
		of the file will be populated into that mongo collection.
- Run `$ seed` to seed your mongodb with all your data from your `/seeds` folder.

**Note**: Every time you run `$ seed` it will blow away all the data in your collections and re-populate them with whatever is in your `/seeds` directory.

Enjoy!
