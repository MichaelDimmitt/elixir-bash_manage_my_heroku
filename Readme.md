curl -n https://api.heroku.com/account   -H "Accept: application/vnd.heroku+json; version=3"
curl -i -n -X GET https://api.heroku.com/apps -H "Accept: application/vnd.heroku+json; version=3"

RAN into some issues with 
heroku login <<< $"UNAME"\n"PASS"\n
heroku set HEROKU_API_KEY=*''*

if `tty -s`; then echo true; fi

'presourced pasword hash to' >> ./.netrc - this does not work. 
- It appears the server gets updated on logout or a new login which overides previous key
- this thereby invalidates the key you owned previously.

echo UNAME\nPASS\n| heroku login

Things I need to overcome: 
CLI needs to prompt for Password but stdin is not a tty

1) How do I get bash to send a stdin that is not text?

languages dealing with  TypeScript 46.2%   Shell 36.3%   JavaScript 8.8%   NSIS 8.2%   Batchfile 0.5%

https://github.com/hero/cl

so ... tty is not accepted 🤔 , what does their code take as an input?
