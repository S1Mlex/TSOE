# TSOE
MPP Bot script




// ==UserScript==
// @name         .
// @namespace    http://tampermonkey.net/
// @version      1.4
// @description  MPP bot for chat.
// @author       >.<
// @include      multiplayerpiano.net
// @include      mpp.8448.space
// @include      *://multiplayerpiano.com/*
// @include      *://mppclone.com/*
// @icon         https://avatars.mds.yandex.net/i?id=9f0f1cf82e2631cd9d3f1324ac560555_l-5042086-images-thumbs&n=13
// @grant        none
// ==/UserScript==
var adminarray = [];
MPP.client.on("a", function(msg) {
    var asgr = msg.a.split(' ');
    var cmd = asgr[0];
    var input = msg.a.substring(cmd.length).trim();
var d = new Date();
var n = d.toLocaleTimeString();
("The time is: \n"+n);


    //All bot comands: /help /h /owner /name /id /ycolor /time /rname /yes /no /pi /да /нет /kill /spam /cat /dog /meow /uwu /owo /like /dislike /rip /ban /ban1 /ban2 /unban /deadspam /admin /w2g /?
    // /c1 /c2 /c3 /c4 /c5 /c6 /c7 /hi /bye /привет /пока .


    //Commands help: /help /help_(category) /h /h_(category)
    //Commands bot: /owner /name /id /ycolor /yes /no /pi /да /нет /kill /spam /cat /dog /meow /uwu /owo /like /dislike /rip /hi /bye /привет /пока
    //Commands color: /c1 /c2 /c3 /c4 /c5 /c6 /c7 /ycolor
    //Commands admin: /ban /unban /deadspam /w2g /?

// TimeUnit.SECONDS.sleep(1);














// Help commands:

if (cmd == "/help") {
    MPP.chat.send(" 🔎Comands Info🔎 : `/help` (categories: `/info` `/fun` `/smile` `/owner` `/color` `/random`) `/name` `/id` `/ycolor` `/time` `/rname` `/code (code)` |")
}
    if (cmd == "/info") {
    MPP.chat.send(" 🔎Comands Info🔎 : `/help` (categories: `/info` `/fun` `/smile` `/owner` `/color` `/random`) `/name` `/id` `/ycolor` `/time` `/rname` `/code (code)` |")
}
        if (cmd == "/fun") {
    MPP.chat.send(" 😆Comands Fun😆:  `/yes` `/no` `/pi` `/name` `/да` `/нет` `/kill` `/spam` `/cat` `/dog` `/say` |")
}
    if (cmd == "/smile") {
    MPP.chat.send(" 😈Comands Smile😈: `/meow` `/uwu` `/owo` `/like` `/dislike` `/rip` |")
}
            if (cmd == "/color") {
    MPP.chat.send(" 🟢Comands Color🟢: Color rooms `/c1` `/c2` `/c3` `/c4` `/c5` `/c6` `/c7` your color `/ycolor`|")
}
    if (cmd == "/owner") {
    MPP.chat.send(" ❌Comands Owner❌ : `/ban` (0 min) `/ban1` (1 min) `/ban2` (10 min) `/unban` `/deadspam` `/admin` `/w2g` `/?` |")
}
            if (cmd == "/random") {
    MPP.chat.send(" 🎲Comands Random🎲 : `Coming Soon...` |")
}

    //Bot commands

    if (cmd == "/code") {
            if (msg.a.substring(5).trim() !== "18012012") {
MPP.chat.send("❌You entered wrong code...❌")
MPP.chat.send("Code has 8 numbers (Type: 00000000 ; where 0 - number)")
    }}
                if (msg.a.substring(5).trim() == "18012012") {
MPP.chat.send("✔️You entered correct code...✔️")
            }
        if (cmd == "/rname") {
         MPP.chat.send("Room name: " + MPP.client.desiredChannelId )
    }
if (cmd == "/да") {
    MPP.chat.send("Нет")
}
    if (cmd == "/нет") {
    MPP.chat.send("Да")
}
        if (cmd == "/connect") {
MPP.chat.send("Connecting...")
}
    if (cmd == "/cat") {
    MPP.chat.send("https://avatars.mds.yandex.net/i?id=9f0f1cf82e2631cd9d3f1324ac560555_l-5042086-images-thumbs&n=13")
}
        if (cmd == "/dog") {
    MPP.chat.send("https://i.pinimg.com/736x/42/c9/31/42c93187066effa46d1991939870f5f1.jpg")
}
           if (cmd == "/all_bot_commands") {
    MPP.chat.send("All commands of bot: /help /h /owner /name /id /ycolor /time /rname /yes /no /pi /да /нет /kill /spam /cat /dog /meow /uwu /owo /like /dislike /rip /ban /ban1 /ban2 /unban /deadspam /admin /w2g /? /c1 /c2 /c3 /c4 /c5 /c6 /c7 /hi /bye /привет /пока ")
}
if (cmd == "/yes") {
    MPP.chat.send("No")
}
if (cmd == "/kill") {
    MPP.chat.send(msg.p.name + " killed  " + msg.a.substring(5).trim())
}
    if (cmd == "/say") {
    MPP.chat.send(msg.a.substring(5).trim())
}
    if (cmd == "/pi") {
    MPP.chat.send("π = 3.14159265358979323846264338327950288419716939937510... ")
}
    if (cmd == "/meow") {
    MPP.chat.send("🐱")
}
    if (cmd == "/uwu") {
    MPP.chat.send("UwU")
}
    if (cmd == "/owo") {
    MPP.chat.send("OwO")
}
    if (cmd == "/rip") {
    MPP.chat.send("💀")
}
    if (cmd == "/spam") {
    MPP.chat.send("SPAM")
}
        if (cmd == "/spam") {
    MPP.chat.send("SPAM")
}
            if (cmd == "/spam") {
    MPP.chat.send("SPAM")
}
        if (cmd == "/spam") {
    MPP.chat.send("SPAM")
}
    if (cmd == "/name") {
    MPP.chat.send("Your name: " + msg.p.name)
}
        if (cmd == "/spam") {
    MPP.chat.send("SPAM")
}
            if (cmd == "/spam") {
    MPP.chat.send("SPAM")
}
            if (cmd == "/spam") {
    MPP.chat.send("SPAM")
}
            if (cmd == "/spam") {
    MPP.chat.send("SPAM")
}
            if (cmd == "/spam") {
    MPP.chat.send("SPAM")
}
            if (cmd == "/spam") {
    MPP.chat.send("SPAM")
}
            if (cmd == "/spam") {
    MPP.chat.send("SPAM")
}
            if (cmd == "/spam") {
    MPP.chat.send("SPAM")
}
            if (cmd == "/spam") {
    MPP.chat.send("SPAM")
}
            if (cmd == "/like") {
    MPP.chat.send("👍")
}
            if (cmd == "/dislike") {
    MPP.chat.send("👎")
}
    if (cmd == "/привет") {
    MPP.chat.send("ПРИВЕТИКИ!!  " + msg.p.name + "!")
}
    if (cmd == "/пока") {
    MPP.chat.send("Пока:(  " + msg.p.name + "!")
}
if (cmd == "/no") {
    MPP.chat.send("yes")
}
    if (cmd == "/time") {
    MPP.chat.send("The time is: " + n);
}
    if (cmd == "/afk") {
    MPP.chat.send(msg.p.name + "Why you AFK ?:( ")
}
if (cmd == "/id") {
    MPP.chat.send("Your ID:  " + msg.p.id)
}
if (cmd == "/ycolor") {
    MPP.chat.send("Your color:  " + msg.p.color)
}
if (cmd == "/hi") {
    MPP.chat.send("HELLOOO!!  " + msg.p.name + "!")
}
if (cmd == "/bye") {
    MPP.chat.send("Bye:(  " + msg.p.name + " :(")
}


    //Color commands

{
if (cmd == "/c1") {
const RC1 = "#ffffff";
const RC2 = "#000000";

MPP.client.sendArray([{m: "chset", set: {color: RC1, color2: RC2}}])
    MPP.chat.send("Set colors - INNER: #FFFFFF (white) • OUTER: #000000 (black).")
}}
{
if (cmd == "/c2") {
const RC12 = "#1ae40c";
const RC22 = "#000000";

MPP.client.sendArray([{m: "chset", set: {color: RC12, color2: RC22}}])
    MPP.chat.send("Set colors - INNER: #1AE40C (green) • OUTER: #000000 (black).")
}}
{
if (cmd == "/c3") {
const RC13 = "#204fd9";
const RC23 = "#000000";

MPP.client.sendArray([{m: "chset", set: {color: RC13, color2: RC23}}])
    MPP.chat.send("Set colors - INNER: #204FD9 (blue) • OUTER: #000000 (black).")
}}
{
if (cmd == "/c4") {
const RC14 = "#ff0000";
const RC24 = "#000000";

MPP.client.sendArray([{m: "chset", set: {color: RC14, color2: RC24}}])
    MPP.chat.send("Set colors - INNER: #D92020 (red) • OUTER: #000000 (black).")
}}
{
if (cmd == "/c5") {
const RC15 = "#d99620";
const RC25 = "#000000";

MPP.client.sendArray([{m: "chset", set: {color: RC15, color2: RC25}}])
    MPP.chat.send("Set colors - INNER: #D99620 (yellow) • OUTER: #000000 (black).")
    }}
{
if (cmd == "/c6") {
const RC16 = "#000000";
const RC26 = "#000000";

MPP.client.sendArray([{m: "chset", set: {color: RC16, color2: RC26}}])
    MPP.chat.send("Set colors - INNER: #000000 (black) • OUTER: #000000 (black).")
        }}
{
if (cmd == "/c7") {
const RC17 = "#ffffff";
const RC27 = "#ffffff";

MPP.client.sendArray([{m: "chset", set: {color: RC17, color2: RC27}}])
    MPP.chat.send("Set colors - INNER: #FFFFFF (white) • OUTER: #FFFFFF (white).")
}}
    {
if (cmd == "/c8") {
const RC18 = "#ff0000";
const RC28 = "#4a0a10";

MPP.client.sendArray([{m: "chset", set: {color: RC18, color2: RC28}}])
    MPP.chat.send("Set colors - INNER: #FFFFFF (white) • OUTER: #FFFFFF (white).")

    //SECRET ROOM (its admin comand)


}}
if ((adminarray.indexOf(msg.p._id) > - 1) || (msg.p._id == MPP.client.getOwnParticipant()._id)) {
if (cmd == "/?") {
    MPP.chat.send("Secret Room - https://multiplayerpiano.net/?c=Secret%20Room")




    //Admin commands

}}
if ((adminarray.indexOf(msg.p._id) > - 1) || (msg.p._id == MPP.client.getOwnParticipant()._id)) {
if (cmd == "/play") {
    MPP.chat.send("Now Playing: " + msg.a.substring(5).trim() + " .")
    }}
if ((adminarray.indexOf(msg.p._id) > - 1) || (msg.p._id == MPP.client.getOwnParticipant()._id)) {
if (cmd == "/stop") {
    MPP.chat.send("Stopped!")

}}
if ((adminarray.indexOf(msg.p._id) > - 1) || (msg.p._id == MPP.client.getOwnParticipant()._id)) {
if (cmd == "/max_nq") {
    MPP.chat.send("✔️Set!✔️ NQ points - 12000")
}}
    if ((adminarray.indexOf(msg.p._id) > - 1) || (msg.p._id == MPP.client.getOwnParticipant()._id)) {
if (cmd == "/max_nq") {
setInterval(() => {
    MPP.noteQuota.points = 12000;
    MPP.noteQuota.max = 12000;
    MPP.noteQuota.allowance = 12000;
}, 1000);
        }}
if ((adminarray.indexOf(msg.p._id) > - 1) || (msg.p._id == MPP.client.getOwnParticipant()._id)) {
if (cmd == "/unmax_nq") {
    MPP.chat.send("✔️Set!✔️ NQ points - 1200")
}}
    if ((adminarray.indexOf(msg.p._id) > - 1) || (msg.p._id == MPP.client.getOwnParticipant()._id)) {
if (cmd == "/unmax_nq") {
setInterval(() => {
    MPP.noteQuota.points = 1000;
    MPP.noteQuota.max = 1200;
    MPP.noteQuota.allowance = 400;
}, 10000);
}}
if ((adminarray.indexOf(msg.p._id) > - 1) || (msg.p._id == MPP.client.getOwnParticipant()._id)) {
        if (cmd == "/w2g") {
    MPP.chat.send("w2g - https://w2g.tv/?r=m3znsph1fbie76q6db")

}}
if ((adminarray.indexOf(msg.p._id) > - 1) || (msg.p._id == MPP.client.getOwnParticipant()._id)) {
if (cmd == "/ban") {
MPP.client.sendArray([{m: 'kickban', _id: msg.a.substring(5).trim(), ms: 0}])
    MPP.chat.send("User has banned from the room for 0 minutes! ID:" + msg.a.substring(5).trim())
}}
if ((adminarray.indexOf(msg.p._id) > - 1) || (msg.p._id == MPP.client.getOwnParticipant()._id)) {
if (cmd == "/ban1") {
MPP.client.sendArray([{m: 'kickban', _id: msg.a.substring(5).trim(), ms: 60000}])
    MPP.chat.send("User has banned from the room for 1 minutes! ID:" + msg.a.substring(5).trim())
}}
if ((adminarray.indexOf(msg.p._id) > - 1) || (msg.p._id == MPP.client.getOwnParticipant()._id)) {
if (cmd == "/ban2") {
MPP.client.sendArray([{m: 'kickban', _id: msg.a.substring(5).trim(), ms: 600000}])
    MPP.chat.send("User has banned from the room for 10 minutes! ID:" + msg.a.substring(5).trim())
}}
if ((adminarray.indexOf(msg.p._id) > - 1) || (msg.p._id == MPP.client.getOwnParticipant()._id)) {
if (cmd == "/unban") {
MPP.client.sendArray([{m: 'unban', _id: msg.a.substring(7).trim()}])
    MPP.chat.send("User has unbanned from the room! ID:" + msg.a.substring(5).trim())
    }}
    //Have fun :)
                     }) /*msg.a. response end*/
