So I can share my Rubymine Preferences between computers. You're welcome to use them, but they're mainly for my own convenience so your experience may be frequently unpleasant.

I've added most of the preferences I don't care much about to .gitignore.

I setup these preferences on a new machines by doing something like to this:

	mkdir -p ~/Library/Preferences/RubyMine30
	cd ~/Library/Preferences/RubyMine30
	git init
	git remote add origin git@github.com:hiremaga/RubyminePreferences.git
	git fetch
	git branch master origin/master
	# !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
	# WARNING: This step will overwrite your local preferences.
	# !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
	git reset --hard
