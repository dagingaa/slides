##  Closures

<small>A way to do encapsulation in JavaScript</small>

````javascript
var email = {...};
var sendWelcomeEmail = (function () {
    var template = fs.readFileSync("path", { encoding: 'utf-8' });
    var renderTemplate = _.template(template);

    return function (to, roomName) {
        email.sendMultipartMail({
            from: 'feedback@appear.in',
            recipients: [to],
            subject: "appear.in" + roomName + " is yours!",
            text: renderTemplate({ roomName: roomName }),
        });
    };
})();

sendWelcomeEmail("dagingaa@appear.in", "/dagingaa");
````


note:
    Put your speaker notes here.
    You can see them pressing 's'.
